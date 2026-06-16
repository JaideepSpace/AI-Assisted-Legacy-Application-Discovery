CASE STUDY 02 – IMPACT ANALYSIS

====================

OBJECTIVE

---

To evaluate how AI-assisted dependency analysis can identify downstream impact of a regulatory or business change.

BUSINESS SCENARIO

---

A regulatory update requires an increase in **statutory interest rates** applied to overdue taxpayer liabilities.

The change affects:

• Interest calculation rules
• Financial reporting
• Compliance reporting
• Refund processing logic

TRADITIONAL APPROACH

---

Impact analysis requires:

• Reviewing COBOL programs (TXI510, TXL320, TXN520)
• Checking batch dependencies
• Consulting SMEs
• Manual review of reporting logic

Estimated effort: 3–7 days.

AI-ASSISTED APPROACH

---

Using Program Inventory + Data Lineage + Vendor Documentation, AI identifies impacted components.

IMPACTED COMPONENTS

---

Primary Impact:

• TXI510 – Interest Calculation
• TXN520 – Penalty Assessment

Secondary Impact:

• TXL320 – Liability Calculation
• TXP410 – Payment Processing
• TXR610 – Refund Processing

Downstream Impact:

• Statutory Reporting (TXS900)
• Audit Reporting (TXA810)
• Compliance Monitoring (TXC710)

DATA IMPACT

---

• INTEREST_TRANSACTION
• TAX_LIABILITY
• PENALTY_TRANSACTION
• REPORTING_DATA

BUSINESS RISKS IDENTIFIED

---

• Incorrect taxpayer balances
• Regulatory reporting inconsistencies
• Refund miscalculations
• Audit discrepancies

TESTING REQUIREMENTS

---

• Interest calculation validation
• Penalty recalculation verification
• Refund recomputation testing
• Reporting reconciliation

KEY LEARNING

---

Even a single parameter change (interest rate) propagates across multiple functional domains.

AI-assisted impact analysis significantly reduces dependency on manual traceability efforts.

