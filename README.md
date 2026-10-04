# GLP-1 Spending Trends in Medicare Part D

## Business question
How is spending on GLP-1 drugs evolving in Medicare Part D, and where is it concentrated?

## Why this matters
GLP-1s (Ozempic, Wegovy, Mounjaro, Zepbound) are the biggest commercial
story in pharma — Novo Nordisk vs. Eli Lilly, supply constraints, and
payers wrestling over coverage. Understanding where the money flows is
core commercial analytics work.

## Dataset
Centers for Medicare & Medicaid Services (CMS), Medicare Part D
Prescribers by Geography and Drug, Public Use File.
Years: 2022-2024 — https://data.cms.gov/provider-summary-by-type-of-service/medicare-part-d-prescribers/medicare-part-d-prescribers-by-geography-and-drug
- Grain: prescribing aggregated by state and drug
- Note: CMS suppresses cells with fewer than 11 claims (privacy rule)

## Method
1. Filter to GLP-1 drugs (semaglutide, tirzepatide, liraglutide, dulaglutide, exenatide)
2. Standardize brand vs. generic name spellings
3. Handle suppressed small cells (approach documented here when decided)
4. Compute: year-over-year spend growth, spend per beneficiary by state, cost per claim by drug

## Findings
_In progress._

## AI workflow log
_In progress — what AI drafted vs. what was verified by hand._

## Limitations
- Medicare Part D only (excludes commercial insurance and Medicaid)
- Suppressed small cells (see Method)
- Descriptive analysis, not causal
