OVERVIEW
========

This project evaluates how Generative AI can be used to improve knowledge discovery, application understanding, impact analysis, and operational decision support within a large-scale tax processing platform.

The architecture is based on Retrieval-Augmented Generation (RAG) principles where responses are generated using enterprise knowledge sources rather than relying solely on a foundation model's general knowledge.

The objective is to enable users to ask business and operational questions in natural language and receive responses grounded in trusted enterprise documentation.

BUSINESS DRIVERS
================

The architecture was designed to address common challenges associated with large legacy platforms including:

• Limited application knowledge visibility
• SME dependency
• Business rule discovery
• Impact analysis effort
• Data lineage investigation
• Production support investigations
• Modernization assessment activities
• Knowledge management challenges

TARGET USERS
============

The solution is intended to support multiple stakeholder groups.

**Production Support Teams** Require rapid access to operational procedures, dependencies, recovery guidance, and incident history.
**Business Analysts** Require visibility into business functionality, rules, processes, and regulatory impacts.
**Application Architects** Require understanding of application dependencies, interfaces, data flows, and modernization opportunities.
**Project Teams** Require impact analysis, application discovery, and implementation planning support.
**Modernization Teams** Require insights into technical complexity, business functionality, and transformation priorities.

HIGH LEVEL ARCHITECTURE
=======================

The proposed architecture consists of four logical layers.

Knowledge Sources
↓
Knowledge Repository
↓
AI Retrieval Layer
↓
Business Users

KNOWLEDGE SOURCES
=================

The knowledge repository aggregates information from multiple enterprise artifacts.

Sources include:
• Application overviews
• Vendor documentation
• COBOL program inventories
• Copybooks
• Batch schedules
• Operational runbooks
• Incident records
• Data lineage documentation
• Release notes
• Modernization assessment reports

These artifacts represent the institutional knowledge required to understand and operate the platform.

KNOWLEDGE REPOSITORY
====================
A consolidated repository created by aggregating and organizing the above knowledge sources to support AI-assisted retrieval, discovery, and analysis.
The repository acts as the centralized source of information used by the AI retrieval layer.
Information is organized and indexed to enable efficient retrieval across multiple documents.
The repository provides a unified view of operational, technical, and business knowledge that would otherwise be distributed across separate systems and documents.

AI RETRIEVAL LAYER
==================
The AI retrieval layer receives natural language questions from users.
Rather than generating responses from general training data, the retrieval process first identifies relevant information from enterprise documentation.
The retrieved information is then used to generate contextual responses.
This approach helps improve accuracy, traceability, and relevance while reducing the likelihood of unsupported responses.

PROTOTYPE IMPLEMENTATION
========================

The original objective was to evaluate how an AI-assisted knowledge retrieval capability could support application discovery, business rule analysis, impact assessment, and modernization activities using enterprise documentation as the primary knowledge source.

As an initial proof-of-concept, Google NotebookLM was used as the evaluation platform to explore key Retrieval-Augmented Generation (RAG) concepts within a controlled environment.

A synthetic enterprise knowledge repository was created using representative application documentation, program inventories, data lineage records, incident history, and vendor documentation. These knowledge sources were loaded into NotebookLM to simulate an AI-assisted discovery and analysis capability.

The prototype evaluated the ability of AI to retrieve, correlate, and synthesize information across multiple independent knowledge sources rather than relying solely on the foundation model's general knowledge.

The evaluation focused on determining whether AI could provide source-grounded responses to business and operational questions related to:

• Application discovery
• Business rule identification
• Impact analysis
• Data lineage analysis
• Modernization assessment
• Knowledge transfer

The prototype also assessed:
• Multi-document knowledge retrieval
• Cross-document relationship discovery
• Source traceability
• Response relevance
• Knowledge accessibility

The findings demonstrated that AI-assisted knowledge retrieval can significantly improve access to operational and application knowledge within large legacy environments while highlighting the importance of documentation quality, governance controls, and human validation for enterprise adoption.


REPRESENTATIVE USE CASES
=======================

Application Discovery
-------------------
Example Question:
"What modules participate in taxpayer refund processing?"
Expected Outcome:
Identification of related applications, jobs, interfaces, and supporting documentation.

Business Rule Discovery
-----------------------
Example Question:
"How are late-payment penalties calculated?"
Expected Outcome:
Identification of applicable business rules and supporting source references.

Impact Analysis
---------------
Example Question:
"What systems may be impacted by a change to penalty assessment logic?"
Expected Outcome:
Identification of affected applications, jobs, reports, interfaces, and testing considerations.

Data Lineage Analysis
---------------------
Example Question:
"Where is taxpayer status created, updated, and consumed?"
Expected Outcome:
Visibility into upstream and downstream data flows.

MODERNIZATION SUPPORT
=====================
The architecture also supports modernization initiatives by providing improved visibility into:

• Business functionality
• Application dependencies
• Data flows
• Technical complexity
• Knowledge concentration areas
• Candidate modernization opportunities

The approach helps accelerate discovery activities commonly required during transformation programmes.

GOVERNANCE CONSIDERATIONS
=========================
AI-generated responses should be treated as decision-support information rather than authoritative guidance.

Enterprise deployment would require:
• Human validation
• Access controls
• Documentation governance
• Auditability
• Regulatory compliance review
• Operational approval processes

The quality of generated responses remains dependent on the quality and completeness of available documentation.

FUTURE STATE ARCHITECTURE
=========================

A future enterprise implementation could include:
• Agents:
  - AI-assisted Impact Analysis Agent
  - AI-assisted Data Lineage Discovery Agent
  - AI-assisted Application Discovery Agent
  - AI-assisted Modernisation Assessment Agent
• Automated ingestion of vendor documentation, runbooks, incident records and operational documentation
• Continuous updating of enterprise knowledge sources to reflect application and business changes
• Incident management integration
• Enterprise search capabilities
• Role-based access controls

The long-term vision is to establish an AI-assisted knowledge platform that enables faster access to enterprise knowledge while supporting operational efficiency, modernisation planning, and informed decision-making.

ARCHITECTURAL CONCLUSION
=========================
This proof-of-concept demonstrates how Retrieval-Augmented Generation principles can be applied to large legacy environments to improve access to operational and application knowledge.

While the prototype implementation was intentionally lightweight, the evaluation indicates that AI-assisted knowledge retrieval has the potential to reduce investigation effort, improve knowledge accessibility, and support modernization initiatives within complex enterprise platforms.

