# Model QA, sensitivity checks and limitations

**Workbook:** `Dominos_LBO_Financial_Model.xlsx` (13 formula-linked worksheets). **Data cut-off:** 6 November 2026. **Historical sources:** official UK annual and half-year disclosures.

## Verified model output (base case)

- Undisturbed share price / shares: **231p** / **384.868623 million**.
- Market equity capitalisation: **£889.0m**.
- LTM underlying EBITDA: **£136.2m**.
- Hypothetical acquisition EV: **£1,445.9m**.
- New senior debt: **£408.6m**.
- Sponsor equity invested: **£1,083.5m**.
- Exit FY2031 EBITDA and exit net debt: **£176.5m** / **£30.8m**.
- Exit sponsor equity proceeds: **£1,557.4m**.
- Five-year gross sponsor MOIC: **1.4373x**.
- Five-year gross sponsor IRR: **7.525%**.
- Reverse 20%-IRR max target equity price: **£707.1m**.

## Tests actually performed during creation

1. The formula-based model was recalculated using the supported spreadsheet engine. **The model `Checks` sheet reports PASS.**
2. The model totals **Sources = Uses**; equity bridge and exit-value checks were reviewed.
3. A return bridge error was detected and corrected during construction (exit EV and net debt had previously been summed incorrectly), then recalculated.
4. The scenario selector was toggled to **Bear / Base / Bull** and confirmed to reconcile to individually recomputed IRRs; returned to **Base** at export.
5. Initial leverage sensitivities were constructed as dynamic independent cash-flow and debt-case calculations instead of static outputs.
6. The `.xlsx` archive's internal ZIP file CRC integrity check passed. This is **not a substitute for an external model audit**.

## Explicit simplifications / risks

- Market premium, term-loan interest, leverage multiples, financing fees, annual FCF assumptions and exit multiple are **illustrative inputs**; no actual sponsor or lender has proposed these financing terms.
- H1 2026 balance-sheet point-in-time debt is used with a November 2026 closing share price; the date mismatch is disclosed and is a modelling convention, **not** a same-day capitalisation table.
- IFRS 16: the UK franchise model includes head leases and subleases. The simplified enterprise-value bridge uses financial debt and financial cash consistently with underlying EBITDA conventions; a complete buyout diligence process would reconcile all lease obligations/receivables and EBITDA adjustments in detail.
- FY2025 balance sheet comparisons require an IFRS 15 restatement documented in interim results; the workbook includes a bridge rather than silently overriding original audited numbers.
- Five-year operating forecasts and cash-sweep mechanics are management-*independent*, not management guidance. No detailed covenant package, revolving-credit availability draw logic, deferred taxes, closing working-capital adjustment or purchase-price allocation schedule is represented as final legal terms.
- A revenue / EBITDA model of an operating business is **not** a deal feasibility opinion: franchise change-of-control consents, diligence, funding commitments, dividends, public takeover rules and transaction fees could change results dramatically.
- Gross sponsor IRR excludes GP management fees, carried interest and fund-level offsets; it is not net LP IRR.

All reported model results should be rechecked after changing inputs; any retained screenshots/PDFs reflect only the base scenario at creation, not subsequent interactive edits.
