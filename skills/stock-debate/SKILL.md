---
name: stock-debate
description: Bull vs Bear debate on an Indian listed stock (NSE/BSE). A researcher builds a fact sheet from investor presentations, concalls and 5-year financials, then Bull and Bear argue and rebut, and a Judge gives the verdict. Use when the user types /stock-debate <company> or asks for a bull/bear debate on an Indian stock.
argument-hint: "<company name> [rounds]"
---

# Stock debate

Input: `$ARGUMENTS` = company name, optionally followed by a number of rebuttal rounds (default 2). If no company is given, ask for one.

Each agent is a **separate general-purpose subagent** (Agent tool), run one after another, so each argues independently.

## Transcript file

Keep the transcript in `debate_<Company>_<YYYY-MM-DD>.md` in the current working directory (spaces in the company name become `_`). Start it with a title line, then after each subagent returns:

1. **Print its contribution to the user in full** under a heading with the agent's name (subagent output is not shown to the user otherwise).
2. Append it to the transcript file under the same heading, followed by `---`.

Give every subagent the shared rules, its role, and the **absolute path** of the transcript file, with the instruction to read it in full first and not to edit it. Do not paste the transcript into the prompt.

## Shared rules (include in every subagent prompt)

You are part of an equity research debate on an Indian listed company. Use WebSearch/WebFetch for real, current numbers: screener.in, NSE/BSE filings, the company's investor presentations, concall transcripts, annual reports, credit-rating notes. Cite every figure with year/quarter and source. Amounts in INR crore. Never invent numbers; say "not found" instead. Mark figures you calculate yourself as "derived". Return only your final contribution, in markdown.

Also tell every subagent today's date.

## Turn order

1. **RESEARCHER** (neutral analyst): fact sheet: business and segments; last 5 years revenue, EBITDA margin, PAT, operating cash flow, capex, free cash flow, debt/equity, ROE/ROCE, working-capital days; latest quarter; key points and guidance from the latest investor presentation and concall; promoter holding/pledge, FII/DII trend; valuation (P/E, EV/EBITDA, P/B) vs 5-year history and listed peers. Use tables. No opinion.
   - **Banks, NBFCs and insurers:** replace the industrial metrics with advances, deposits/borrowings, NII, NIM, fee income, cost-to-income, PPOP, credit cost, GNPA/NNPA, PCR, slippages, CASA, CRAR/CET1, LDR, ROA, ROE, BV/ABV per share, and value on P/B, P/ABV and sum-of-the-parts for listed subsidiaries. Insurers: VNB margin, combined ratio, solvency, embedded value.
   - **Recent demergers, mergers or renamings:** tell the Researcher to verify the corporate structure and cover each listed entity separately, saying which entity each number refers to.
2. **BULL** opening: the strongest investment thesis from the facts, addressing the obvious objections head-on.
3. **BEAR** opening: the strongest anti-thesis (accounting quality, cash conversion vs profit, governance, related-party deals, debt, cyclicality, competition, valuation; for lenders: provisioning, funding, asset quality, regulatory issues) and a rebuttal of the Bull.
4. Repeat for each rebuttal round: **BULL** rebuttal, then **BEAR** rebuttal. Each attacks the other's specific latest claims with data (searching for new numbers if needed) and concedes points that are true. Name the key disputes from the previous turn in the prompt so each round stays focused.
5. **JUDGE** (CIO chairing the meeting; search only if a disputed number decides the case): who argued better and why, points each side won, unresolved questions, a 1-10 conviction score (state the scale), and monitorables that would change the view. End with "Educational discussion, not investment advice."

## Finish

Make sure the transcript file holds every contribution, then tell the user its path.
