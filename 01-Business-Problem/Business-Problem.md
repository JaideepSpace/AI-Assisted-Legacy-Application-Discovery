Business Problem
================

Background
----------

The Tax Processing Platform (TPP) is a mission-critical government revenue system responsible for tax return processing, taxpayer account maintenance, compliance validation, refund calculation, payment processing, audit support, and regulatory reporting.

The platform consists of more than 700 COBOL components, including both online and batch-processing modules, along with copybooks, JCL, DB2 objects, interfaces, and operational procedures.

Application development and maintenance are performed by an external software vendor. Internal teams are responsible for implementation, production support, release management, operational stability, and modernization planning.

Over time, significant business and technical knowledge has become distributed across source code, vendor documentation, release notes, operational runbooks, incident records, and support procedures.

As a result, obtaining a complete understanding of application behavior often requires extensive investigation across multiple knowledge sources.


Current Challenges
==================

Challenge 1 – Business Rule Discovery
-------------------------------------
Critical tax-processing rules are embedded within hundreds of COBOL modules and supporting documentation.

Examples include:
* Tax liability calculation
* Refund eligibility determination
* Penalty assessment
* Interest calculation
* Compliance validation

Understanding these rules frequently requires detailed code analysis and consultation with vendor specialists.

Challenge 2 – Change Impact Analysis
------------------------------------
Regulatory and legislative changes occur regularly and often require modifications across multiple online and batch-processing components.

Determining the full impact of a change requires identification of:
* Affected COBOL modules
* Batch jobs
* Online transactions
* Interfaces
* Reports
* Database objects
* Downstream business processes

This analysis is largely manual and dependent on SME knowledge.

Challenge 3 – Application Discovery
-----------------------------------
The platform contains hundreds of interconnected components developed over many years.

Operational and project teams often need answers to questions such as:
* Which modules perform refund calculations?
* Which programs update taxpayer accounts?
* What business functions are supported by a specific component?
* Which batch streams are involved in annual tax processing?

Finding these answers can be time-consuming and inconsistent.

Challenge 4 – Data Lineage Visibility
-------------------------------------
Taxpayer information flows through numerous online transactions, batch processes, interfaces, and reporting systems.

Understanding how a particular data element is created, updated, transformed, and consumed across the platform requires investigation of multiple technical artifacts.

Limited visibility increases risk during change implementation and modernization activities.

---

Challenge 5 – SME Dependency
----------------------------
Knowledge of application behavior is concentrated among a small number of experienced personnel and vendor specialists.

This creates challenges related to:
* Knowledge transfer
* Staff turnover
* Incident response
* Change implementation
* Modernization planning

Challenge 6 – Production Support Efficiency
------------------------------------------
During production incidents, support teams often need to quickly determine:
* Business impact
* Upstream and downstream dependencies
* Recovery options
* Affected taxpayer services
* Potential regulatory impacts

Relevant information is typically spread across multiple documents and systems.

Challenge 7 – Modernization Planning
------------------------------------
The organization requires improved visibility into application complexity, technical debt, business functionality, and system dependencies to support future modernization initiatives.

Current assessment activities require significant manual effort and extensive SME involvement.

Desired Future State
====================
Establish an AI-assisted knowledge discovery capability that enables operational teams, analysts, architects, modernization teams, and business stakeholders to retrieve and analyze information across technical and business artifacts using natural language queries.

The solution should support:
* Application discovery
* Business rule extraction
* Change impact assessment
* Data lineage analysis
* Production support investigations
* Modernization planning
* Knowledge management

while maintaining appropriate governance controls and human validation processes.

Project Objective
=================
Evaluate whether Generative AI and Retrieval-Augmented Generation (RAG) concepts can improve access to operational and application knowledge within a large-scale tax processing environment by providing source-grounded responses based on existing documentation and application artifacts.
Evaluate whether Generative AI and Retrieval-Augmented Generation (RAG) concepts can improve access to operational and application knowledge within a large-scale tax processing environment by providing source-grounded responses based on existing documentation and application artifacts.
