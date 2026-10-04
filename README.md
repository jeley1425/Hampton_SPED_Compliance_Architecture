Hampton City Public Schools: Special Education Compliance Audit & Resource Pipeline

Executive Document & Architecture Overview
Public school systems operate under rigid federal timelines mandated by the Individuals with Disabilities Education Act (IDEA). Failure to finalize specialized student eligibility evaluations within the strict 60-day window from parental consent introduces severe vulnerabilities: immediate state regulatory sanctions, structural funding freezes, and costly due process legal arbitrations. 

This repository houses an end-to-end data engineering and prescriptive optimization pipeline anchored explicitly within the institutional architecture of Hampton City Public Schools (HCPS). By processing student case registries, the pipeline automatically synthesizes raw case timelines into a multi-factor compliance risk index, rolls individual data boundaries up to a building level, utilizes unsupervised machine learning to isolate critical compliance bottlenecks, and executes an automated caseworker redistribution model to eliminate district-wide financial and legal exposure.

Technical Architecture & Core Subsystems
The production pipeline implements a 5-phase data science lifecycle engineered in Python:

Phase 1: Compliance Ingestion Schema – Developed a data connector ingesting 500 active, multi-variable student tracking logs distributed across 9 regional Hampton secondary campuses (including Bethel, Phoebus, Hampton, and Kecoughtan High Schools).
Phase 2: Regulatory Feature Engineering – Vectorized a mathematical timeline variance module calculating precise days over the federal mandate. This is synthesized into a composite-Legal Risk Score that balances individual caseworker overloads against parent communication metrics, while mapping a \$7,500 state mediation cost baseline directly to out-of-compliance files.
Phase 3: Unsupervised Building-Level Aggregation – Aggregated individual case-level granular rows (capturing individual student anomalies) into a centralized campus summary matrix. Applied a Scikit-Learn geometric `KMeans` clustering algorithm to automatically segment campuses into distinct operational risk tiers.
Phase 4: Prescriptive Resource Allocation – Built an automated resource triage matrix that mathematically isolates the highest-risk campus cluster and triggers an emergency caseworker reallocation protocol, targeting staff deployments strictly to backlogged buildings.
Phase 5: High-Dimensional Executive Dashboard – Engineered an interactive scatter and bubble index overlaying aggregate campus risk scores directly against total litigation exposure, providing superintendents with an immediate, clear view of district operational bottlenecks.

Real-World Operational Insights (Case File Mechanics)
To maintain strict compliance with federal data privacy mandates under the Family Educational Rights and Privacy Act (FERPA) and HIPAA regulations, this pipeline utilizes a high-fidelity simulated dataset that perfectly mimics real-world district parameters. 

In production, the model operates on granular student rows before aggregating them to building summaries. For example, during initial data indexing, individual campuses will show multiple case entries reflecting actual school operations:
Case HAMP-SPED-10001 (Eaton Middle School):** Identifies a student file safely within the legal timeline margin, resulting in a low Legal Risk Score (21.9) and \$0 in corporate liability exposure.
Case HAMP-SPED-10002 (Eaton Middle School): Automatically catches a severe timeline breach where a student evaluation has crossed the 60-day limit under an overloaded caseworker, driving the Legal Risk Score to 48.3 and instantly flagging a \$7,500 financial exposure risk.

The clustering mechanism takes these individual variations, rolls them into campus metrics, and isolates systemic building backlogs so district directors can intervene before mediation triggers.

Tech Stack & Framework Infrastructure
Programming Language: Python 3
Development Environment: Google Colab / Jupyter Notebooks
Core Core Libraries: Scikit-Learn (StandardScaler, KMeans), Pandas, NumPy, Matplotlib, Seaborn
