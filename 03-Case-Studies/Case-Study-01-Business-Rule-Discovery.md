CASE STUDY 01 – BUSINESS RULE DISCOVERY

====================

OBJECTIVE

---

To evaluate how AI-assisted knowledge retrieval can identify and explain embedded business rules across distributed legacy documentation in the Tax Processing Platform (TPP).

BUSINESS SCENARIO

---

A business analyst needs to understand how **taxpayer penalty calculation** is implemented within the platform.

The rule is not documented in a single place and is distributed across:

• Vendor documentation
• COBOL program logic (TXN520, TXI510)
• Control tables
• Batch processing rules

TRADITIONAL APPROACH

---

Without AI support, understanding the business rule requires:

• Manual COBOL code review
• SME consultation
• Cross-referencing vendor manuals
• Reviewing batch jobs and control tables

Estimated effort: 2–5 days depending on SME availability.

AI-ASSISTED APPROACH

---

Using a Retrieval-Augmented Knowledge approach, relevant information is correlated across:

• Vendor Documentation (Penalty Assessment Rules)
• Program Inventory (TXN520, TXI510)
• Data Lineage (PENALTY_TRANSACTION)
• Incident History (TPP-2025-142)

DISCOVERED BUSINESS RULE

---

Penalty Calculation Logic:

• Penalty is triggered for late filing or late payment
• Penalty is calculated as a percentage of outstanding liability
• Interest (TXI510) is calculated before penalty application
• Compliance flags may override penalty application in exception cases
• Penalty is stored as PENALTY_TRANSACTION and fed into reporting systems

DEPENDENCIES IDENTIFIED

---

• Liability Calculation (TXL320)
• Interest Calculation (TXI510)
• Compliance Management (TXC710)
• Control Tables (Penalty Rates)

BUSINESS IMPACT

---

Understanding this rule enables:

• Faster regulatory change implementation
• Reduced SME dependency
• Improved test coverage
• Faster compliance validation

KEY LEARNING

---

Embedded business rules exist across multiple disconnected artifacts and require cross-document correlation to reconstruct accurately.

AI significantly reduces dependency on manual code inspection.

