# Net Worth Tracker — Fictional Portfolio Demo

**Public portfolio showcase — October 26, 2026.**

This repository stores the reviewed case study, walkthrough, verification report and five screenshots. It does not contain the original personal workbook, a downloadable workbook, source snapshots or raw audit files. See [Public release: meaning and scope](PUBLIC_RELEASE.md) for what this public showcase includes.

A Google Sheets project that connects day-to-day transactions with cash balances, allowances, fiscal-year reporting and investment analysis. The demonstration preserves the structure of a personal tracking system while using fictional accounts, institutions, transactions, balances, securities, prices and benchmarks.

The scenario is fixed as of **October 25, 2026**. Its values demonstrate the model; they are not personal financial records, market observations or investment recommendations.

## Start here

- [Portfolio case study](case-study.md): the problem, approach, design decisions, features and project value.
- [Walkthrough](walkthrough.md): five captured views with captions and a short demonstration script.
- [Verification and privacy review](verification-and-privacy.md): completed checks, calculation scope and the ownership/history limits that remain.
- [Public release: meaning and scope](PUBLIC_RELEASE.md): what becomes public, what is included and what remains separate.

**Start the project tour:** [Explore the fictional tracker walkthrough](walkthrough.md). A live workbook destination is intentionally not included in this documentation package.

![Fictional net worth dashboard](screenshots/dashboard.jpg)

## What the workbook demonstrates

| Area | Representative functionality |
| --- | --- |
| Dashboard | Connected views of assets, liabilities, spending, cash and fiscal trends |
| Transaction ledgers | Separate records for expenses, income, transfers, card payments, refunds, adjustments and investment trades |
| Allowances | Effective-dated rules with Full, Positive Only, None and Capped carryover policies |
| Fiscal reporting | A September 21–September 20 fiscal calendar, account balances and monthly activity |
| Registries | Account, category and security definitions used consistently by the ledgers and reports |
| Investment analysis | Holdings, average cost, realized and unrealized gains, dividends, cashflow returns and rebalancing |
| Benchmarking | Two fictional index series for exploring monthly and cumulative comparisons |
| Supporting models | Savings and health-account ledgers, cross-border records and fixed fictional currency conversion |
| Quality checks | Reconciliation and validation views designed to surface inconsistent entries |

The workbook keeps input records separate from calculations and presentation. Dashboard totals can be traced back to ledger entries, registry keys and date-based rules. Changing a valid fictional input is intended to update the dependent views.

## Calculation conventions

- Investment quantities and prices come from a deterministic fictional scenario. The demo does not need a live market-data feed.
- Holdings use an average-cost calculation. Purchases, sales, fees and dividends remain distinct transaction types.
- Monthly portfolio returns use cashflow-based XIRR. Linking those monthly returns is a useful comparison series, but it is not a true cashflow-neutral time-weighted return.
- The benchmark lines show fictional index growth. Their growth rates are not cashflow-matched benchmark XIRRs and should not be presented as investment outperformance.
- The October 25 scenario includes current holdings; completed-month performance ends September 30, 2026.
- Currency rates are fictional fixture inputs. The workbook is an analytical project demonstration, not a source of current exchange rates.

## Reviewed screenshots

| View | What it shows |
| --- | --- |
| [Dashboard](screenshots/dashboard.jpg) | Fictional balances, current fiscal spending and the scenario notice |
| [Spending charts](screenshots/spending-charts.jpg) | Monthly external inflow and spending versus available allowance |
| [Fiscal year](screenshots/fiscal-year.jpg) | Fiscal calendar, income, spending and reporting scope |
| [Investments](screenshots/investments.jpg) | Fictional holdings, allocation and synthetic price availability |
| [Monthly performance](screenshots/monthly-performance.jpg) | Portfolio XIRR and fictional benchmark comparisons |

## Verification and privacy status

The original personal workbook is outside this release and was left unchanged. The separately approved copy was checked across 59 sheets, including 42 hidden sheets. A native scan covered 420,885 entered cells; formula repairs were re-read, and the final export scan found no cached formula errors, active external data calls, cell/formula URLs or external package relationships. No known original financial records remained in the reviewed current contents.

A $10 expense scenario propagated correctly and was restored. Five fiscal selections, ten allowance-policy fixtures, all 26 allowance rules and 33 independently recomputed monthly investment-return results passed. Current balances include the fictional India accounts; historical fiscal snapshots cover the listed US accounts.

The copied script is inert and its obsolete run button has been removed. **Google ownership information and earlier workbook/script revisions have not been erased or certified anonymous.** The detailed report explains these limits and distinguishes reviewed current contents from platform history. Five representative views were checked visually; the review does not claim individual visual inspection of every chart.

Anyone can view this repository, case study, walkthrough and screenshots without an invitation. The existing copied workbook's sharing settings and the portfolio website were left unchanged.

## Release contents

The repository contains the case study, walkthrough, verification report, release-scope document and reviewed screenshots. Private source exports, prior snapshots, raw audit files, local credentials and internal working files stay outside it.

This public showcase is available directly from the repository. No version tag or formal GitHub Release is needed to view it.
