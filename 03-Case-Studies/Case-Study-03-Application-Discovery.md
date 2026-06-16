CASE STUDY 03 – APPLICATION DISCOVERY

====================

OBJECTIVE

---

To evaluate how AI-assisted knowledge retrieval can map business questions to relevant application components in a large-scale legacy system.

BUSINESS SCENARIO

---

A support team asks:

“What modules are involved in taxpayer refund processing?”

In a system with 700+ COBOL programs, this is not directly documented.

TRADITIONAL APPROACH

---

Requires:

• Searching program inventories
• Reviewing batch schedules
• SME consultation
• Manual cross-referencing

Estimated effort: hours to days depending on complexity.

AI-ASSISTED APPROACH

---

Using Program Inventory and Vendor Documentation, AI identifies:

REFUND PROCESSING ECOSYSTEM

---

Core Program:

• TXR610 – Refund Processing

Supporting Components:

• TXP410 – Payment Reconciliation
• TXL320 – Liability Calculation
• TXC710 – Compliance Management

Data Dependencies:

• REFUND_TRANSACTION
• TAX_LIABILITY
• PAYMENT_TRANSACTION

Batch Dependencies:

• Refund Batch Stream (Nightly Processing Cycle)

RELATED BUSINESS PROCESSES

---

• Tax Return Processing
• Compliance Validation
• Payment Reconciliation
• Regulatory Reporting

BUSINESS VALUE

---

• Faster application mapping
• Reduced SME dependency
• Improved onboarding efficiency
• Better system understanding for change requests

KEY LEARNING

---

Application discovery in legacy systems requires correlation across programs, data, and batch processes rather than relying on single-source documentation.

