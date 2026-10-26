# Net Worth Tracker

**A connected financial tracking system in Google Sheets, demonstrated with fictional data.**

*Portfolio documentation. Scenario dated October 25, 2026; verification completed October 26, 2026. Stored in the private GitHub documentation package.*

## Project summary

I developed a personal financial tracking system that connects transactions, account balances, spending allowances, fiscal reporting and investment analysis in Google Sheets. The goal was to make each summary traceable to its underlying records and rules.

For the portfolio demonstration, I preserved the workbook’s architecture and replaced financial inputs and stored histories with a fictional scenario. The result demonstrates the working model without relying on personal financial records or live market feeds.

## Problem

A useful balance dashboard needs reliable records underneath it. Transfers can appear as spending, refunds can distort category totals, and investment purchases can be confused with changes in wealth. A non-calendar fiscal year adds date rules, while allowances need explicit treatment of unused and overspent amounts.

Presenting the project also required reviewing hidden calculations and stored histories: deleting visible balances alone would not produce a trustworthy public demonstration.

## Approach and design challenges

I separated input ledgers, shared registries and calculation/reporting views. Expenses, income, transfers, card payments, refunds and investment activity retain distinct meanings. Account, category and security definitions let those records feed consistent summaries.

Fiscal reporting follows a September 21–September 20 calendar. Allowances use effective-dated rules with Full, Positive Only, None and Capped carryover policies. This makes period boundaries and policy changes explicit instead of embedding them in isolated formulas.

Investment views connect trades with holdings, average cost, dividends, returns and allocation targets. The demonstration uses deterministic fictional prices and two fictional benchmark series. Monthly portfolio returns use cashflow-based XIRR; linked monthly XIRRs are labeled accurately and are not described as a true time-weighted return. Benchmark index growth is not presented as a cashflow-matched comparison or evidence of outperformance.

Current consolidated balances include fictional India accounts. Historical fiscal snapshots cover the listed US accounts. Both scopes are labeled so a viewer can interpret the figures correctly.

## Main features

- A dashboard connecting net worth, liquidity, spending and fiscal trends.
- Structured transaction ledgers and shared account/category registries.
- Configurable allowances with four carryover policies.
- Fiscal-year reporting with monthly activity and opening/closing balances.
- Investment holdings, gains, dividends, monthly cashflow returns and rebalancing.
- Validation and reconciliation views that surface inconsistent entries.

## Verification and impact

Independent calculations matched all 33 completed monthly investment periods. Fiscal boundary scenarios and a temporary expense change were checked in the live workbook, with test inputs restored. The content review covered visible and hidden sheets, formulas, chart labels, named ranges, links and scripts.

The project demonstrates spreadsheet data modeling, formula design, reconciliation and reporting through an inspectable working example. Its value is the connection between records, rules and summaries; I do not claim measured time savings, financial gains or commercial adoption.

Current-content checks do not erase Google ownership information or earlier file/script revisions. Those limits are documented separately in the [verification and privacy report](verification-and-privacy.md).

## Explore the fictional demo

**[Explore the fictional tracker walkthrough](walkthrough.md)**

Follow the five captured views from dashboard to spending, fiscal reporting, holdings and monthly performance. An interactive workbook link will be added only as part of a separately reviewed demo release; see [release scope](PUBLIC_RELEASE.md).
