# Verification and privacy review

**Reviewed October 26, 2026. Current-content cleanup complete; documentation approved for private GitHub storage.**

This report concerns the approved **Net Worth Tracker Public** copy. The original personal tracker was treated as strictly read-only. Its contents and permissions were not changed. The copy's existing anyone-with-link reader setting was left unchanged, as requested.

The demonstration uses fictional financial inputs. Prices and balances are based on a scenario through **October 25, 2026**; completed-month investment performance ends **September 30, 2026**. The workbook is a native Google Sheets demonstration. Its inspection export is not a separately certified Excel product.

## What was checked

| Surface | Scope and result |
| --- | --- |
| Workbook architecture | 59 sheets reviewed, including 42 hidden supporting sheets; 47 chart specifications and 11 internal named ranges inspected |
| Native cells | A bounded live scan covered 420,885 entered cells: 405,315 formulas and 15,570 constants. Later edits were re-read and included in the final export review. |
| Financial inputs | Fictional account and institution names, transaction text, trades, prices, balances, fiscal histories, allowances and currency rates replaced the copied scenario. Historical residual values and narrative cells were reviewed as well as visible inputs. |
| Formulas | Two errors found by the live scan were repaired: a malformed remittance formula and an account-list formula blocked by a leftover constant. Both were re-read successfully. The final export contained no cached formula errors. |
| External data | No actual external import, market-data, web-service or image-fetch function calls were found in the final formula scan. No URLs were found in cell values or formulas. Unused source-choice vocabulary is not an active feed. |
| Navigation and identifiers | Remaining navigation links use internal sheet fragments. Registry keys and sheet/chart identifiers support the model; they are not financial account numbers or links to the original workbook. |
| Notes, links and comments | Cell notes and copied rich-text links were cleared. The final Drive comment check returned zero comments, including deleted comments, with no additional results page. |
| Export package | No external package relationships, external-link parts, comment parts, VBA project or custom XML parts were found. The export contained no core-properties author record. |
| Protections | Copied editor-specific protection settings were replaced with warning-only protections. |
| Apps Script | The bound script's current code was replaced with an inert comment. The editor showed no runnable functions, and the inspected project had zero triggers, deployments and script properties. The obsolete GO! script button was removed and the saved workbook was re-opened successfully. |
| Sharing | A final read confirmed anyone-with-link reader access plus the existing owner. No sharing change was made. |

No known original financial records remained in the reviewed current contents after replacement, residual-value checks and the final export comparison. This is an evidence-based current-content conclusion, not a claim that the platform's entire history has been erased.

## Functional verification

| Check | Observed result |
| --- | --- |
| Expense propagation | Increasing one fictional expense by $10 raised fiscal spending and the card liability by $10, reduced net worth by $10 and reduced the applicable allowance balance by $10. The input and dependent results were restored. |
| Fiscal-year selection | Five opening/closing selections matched independently generated boundary balances. The selector was restored to FY 2026–27 / Current. Future closing balances remain blank. |
| Allowances | All 26 populated rules validated. Ten policy fixtures passed, including Full, Positive Only, None, Capped, negative carry, proration and year transitions. |
| Core transaction feed | The 93-row fictional feed reconciled with unique identifiers and no untracked entries. |
| Investments | Independent recomputation matched all 33 completed monthly cashflow/XIRR results within approximately 9.1 × 10⁻¹³. Holdings, dividends, realized gains and model cash balances were also checked. |
| Native quality checks | Populated ledger validations passed and the workbook's system-health checks reported healthy after repairs. |

### Selected fictional reference values

These numbers are test fixtures, not personal results or investment claims.

| Reference | Verified value |
| --- | ---: |
| Current assets | $118,426.49 |
| Current liabilities | $75.00 |
| Current net worth | $118,351.49 |
| Current fiscal-year spending | $1,420.00 |
| Main investment holdings used by the performance model | $6,542.48 |
| FY 2023–24 closing net worth, listed US accounts | $46,186.65 |
| FY 2024–25 closing net worth, listed US accounts | $93,884.92 |
| FY 2025–26 closing net worth, listed US accounts | $114,117.17 |

Current consolidated totals include the fictional India accounts. Historical fiscal snapshots cover the listed US accounts. That scope difference is stated in the workbook and portfolio documents. The fiscal calendar runs September 21 through September 20.

Monthly portfolio returns use cashflow-based XIRR. Linking those monthly returns does not produce a true cashflow-neutral time-weighted return. The two benchmark lines are fictional index-growth series, not cashflow-matched benchmark XIRRs. Neither the charts nor this review support a claim of investment outperformance.

## Visual review

Five final screenshots show the dashboard, spending charts, fiscal-year view, investments and monthly benchmark comparisons. Chart titles identify the fictional benchmarks, the investment view confirms synthetic prices are available, and dashboard/fiscal notices explain the scenario and reporting scope.

The screenshots were captured from the rendered workbook and cropped to worksheet content, excluding the signed-in account controls. Representative views were checked visually; this does not claim that every one of the 47 charts received an individual pixel-level review.

## Privacy limits that remain

1. **Ownership identity:** the existing Google file still belongs to its current owner. A current-cell cleanup does not anonymize Google account ownership or all platform metadata. The metadata connector did not expose every requested description/custom-property field, so those fields are not certified absent.
2. **Earlier revisions:** this was an in-place cleanup of a copy. Earlier workbook revisions and Apps Script revisions were not deleted or proven empty. They must not be described as sanitized by the current-content audit.
3. **Private working evidence:** earlier snapshots and exports remain outside this review package. They must not be uploaded with documentation or included in a repository.
4. **Release scope:** this review package contains only documentation and reviewed images. A new downloadable workbook or newly published live destination requires its own final artifact review. A fresh reconstruction from audited synthetic content would avoid carrying forward this copy's earlier revisions; its new ownership/metadata would still need review.

The existing copy is suitable for reviewing the fictional functionality. It should not be advertised as an anonymous, history-free file. The remaining release decision is whether to use the existing reviewed copy with these limits or prepare a fresh publication artifact before a new portfolio release.

## Evidence and release boundary

The final inspection export was re-fetched after the script-button removal. Its parsed cell formulas and values matched the prior checked export, and its privacy/package scan remained clean. Its SHA-256 is `52e33d5335e7adf79887b7527b4abc0a47f7a859a3d2d5dc223e0bf40168551f`. This hash identifies private audit evidence; the export is intentionally excluded from this package.

Native readbacks, scenario-test records and inspection exports are retained locally outside this repository. The reviewed documentation and screenshots are stored in private GitHub. No formal GitHub Release, public repository, portfolio website update or new interactive workbook distribution is included in this upload. See [public release scope](PUBLIC_RELEASE.md).
