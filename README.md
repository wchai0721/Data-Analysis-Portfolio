# Wen Chai - Data Analyst Portfolio
## About

Hi, I'm Wen! I'm a healthcare strategy and analytics professional with 15+ years of experience spanning consulting, biotech venture building, and translational research. I currently work as a Product Owner and Neuroscientist at the Parr Lab/University of Minnesota (UMN) Neurosurgery, where I bridge the bench and the boardroom: designing organoid experiments and managing cell banks used across labs, while also authoring federal and state grant proposals (e.g. R01, R21, SCITBI) and translating multi-institutional research into executive briefings, roadmaps, and funding narratives for senior leaders across Mayo Clinic, UMN, and industry partners.

My background sits at the intersection of science, business, and analytics. I hold an MBA in Business Analytics and Medical Industry Leadership from the Carlson School of Management and have applied that training across healthcare consulting (Slalom), startup commercialization (Sarcio), and federally funded research programs. I'm fluent working across R&D, clinical, commercial, and operational teams — structuring ambiguous problems, synthesizing complex data, and communicating clearly to stakeholders at every level.

This repository reflects my hands-on work in data analysis, visualization, and modeling — built to complement the strategic and scientific foundation I've developed throughout my career. I'm especially interested in projects at the intersection of healthcare, data, and decision-making.

My CV is available as a PDF.

## Table of Contents

[About](#about)

[Projects](#projects)
- Python + SQL
  - [SCI Clinical Trial Landscape Analysis](https://github.com/wchai0721/Data-Analysis-Portfolio/blob/main/README.md#spinal-cord-injury-clinical-trial-landscape-analysis)
  - [Oncology In Vitro Clinical Trial Landscape Analysis](https://github.com/wchai0721/Data-Analysis-Portfolio/blob/main/README.md#oncology-in-vitro-clinical-trial-landscape-analysis)
- Python + Web
  - [Dopamine Menu Generator](https://github.com/wchai0721/Data-Analysis-Portfolio/blob/main/README.md#dopamine-menu-generator)
- Python + SQL + Tableau
   - [Pittsburgh Trauma Medical Center — ED Shift Analytics](https://github.com/wchai0721/Data-Analysis-Portfolio/blob/main/README.md#pittsburgh-trauma-medical-center--ed-shift-analytics)
- Excel + Tableau
  - [GreenTech Recycling Operations Dashboard](https://github.com/wchai0721/Data-Analysis-Portfolio/blob/main/README.md#greentech-recycling-operations-dashboard)
- Excel
   - [iPSC Cell Line Bank – Product Pricing & Revenue Model](https://github.com/wchai0721/Data-Analysis-Portfolio/blob/main/README.md#ipsc-cell-line-bank--product-pricing--revenue-model)
   - [iPSC Cell Line Bank – New Product Introduction (NPI) Launch Tracker](https://github.com/wchai0721/Data-Analysis-Portfolio/blob/main/README.md#ipsc-cell-line-bank--new-product-introduction-npi-launch-tracker)
- Power BI
- Notion
- R
  
[Education](#education)
  
[Certificates](#certificates)
  
[Contact](#contact)

## Projects

### Spinal Cord Injury Clinical Trial Landscape Analysis

**Code:** [sci_analysis.ipynb](https://github.com/wchai0721/Projects/blob/8766daa737c4918d22b2f354da6cd209d54129d8/sci_analysis.ipynb)

**Data source:** [AACT](https://aact.ctti-clinicaltrials.org)

**Goal:** To identify structural patterns in SCI trial design, intervention types, and phase progression, and to surface translational bottlenecks in the clinical pipeline.

**Description:** The project analyzed 939 registered clinical trials for spinal cord injury using the AACT (Aggregate Analysis of ClinicalTrials.gov) database — a publicly available PostgreSQL database maintained by the Clinical Trials Transformation Initiative. The project involved connecting to a live remote database, querying and joining multiple relational tables, performing exploratory data analysis across trial volume, intervention categories, and phase distribution, and visualizing trends over a 35-year registration period (1989–2026).

**Technology:** Python, Pandas, SQLAlchemy, Seaborn, Matplotlib, PostgreSQL.

**Skills:** SQL querying, relational database joins, data cleaning, exploratory data analysis, data visualization.

**Results:** Analysis revealed that device and behavioral interventions dominate the SCI trial landscape, while biological interventions (including cell-based therapies) represent only 4.4% of registered trials despite growing preclinical interest. Phase progression analysis showed that only ~2% of phased trials reach Phase 3, indicating a steep translational attrition funnel. Trial volume has grown steadily since 2003 with a notable spike in 2025.

### Oncology In Vitro Clinical Trial Landscape Analysis

**Code:** [oncology_landscape.ipynb](https://github.com/wchai0721/Projects/blob/main/oncology_landscape.ipynb)

**Data source:** [AACT](https://aact.ctti-clinicaltrials.org)

**Goal:** To map the global oncology in vitro clinical trial landscape, identify competitive positioning patterns across sponsors and geographies, and surface intervention trends relevant to product strategy at a preclinical CRO.

**Description:** The project analyzed registered clinical trials at the intersection of oncology and in vitro research using the AACT (Aggregate Analysis of ClinicalTrials.gov) database — a publicly available PostgreSQL database maintained by the Clinical Trials Transformation Initiative. The cohort was defined by dual filtering: oncology-related conditions (cancer, tumor, carcinoma, neoplasm, leukemia, lymphoma) combined with in vitro methodology keywords (cell line, organoid, spheroid, xenograft, ex vivo). The project involved connecting to a live remote database, querying and joining multiple relational tables, and performing exploratory data analysis across trial volume, sponsor landscape, phase distribution, intervention types, and geographic distribution.

**Technology:** Python, Pandas, SQLAlchemy, Seaborn, Matplotlib, PostgreSQL.

**Skills:** SQL querying, relational database joins, cohort definition, exploratory data analysis, data visualization, competitive intelligence analysis.

**Results:** Analysis revealed that academic and government institutions dominate the oncology in vitro trial landscape (70.1% other academic, 23.9% NIH), with industry sponsors accounting for only 5.9% of registered trials. Biological and drug interventions lead equally (~229 and 225 trials respectively), with biological trials showing the strongest post-2015 growth trajectory driven by immunotherapy and cell therapy pipelines. Trial volume tripled between 2015 and 2023, peaking at 61 registrations. The US and China account for over half of all trial activity, with emerging Asia-Pacific presence in South Korea, Singapore, and Taiwan.

### Dopamine Menu Generator

**Code:** [dopamine-menu/](https://github.com/wchai0721/Projects/tree/main/dopamine-menu) · [README](https://github.com/wchai0721/Projects/blob/main/dopamine-menu/README.md) · [APP](https://dopamine-menu-o3nl.onrender.com/)

**Data source:** Primary literature (positive psychology research, 2015–2023)

**Goal:** To generate personalized, evidence-backed restorative activity recommendations based on a user's current mood, available time, and energy level.

**Description:** The project built a two-interface Python tool — a CLI and a Flask web app — that scores and ranks restorative activities using a custom recommendation engine. Each activity in the database is grounded in positive psychology research (Seligman, Csikszentmihalyi, Fredrickson, Pennebaker, and others) and tagged with psychological mechanism, mood affinities, energy requirements, and a concrete behavioral tip. The scoring engine applies weighted bonuses for mood match, energy alignment, and time fit, with hard filters that remove incompatible activities before ranking.

**Technology:** Python, Flask, HTML/CSS/JavaScript.

**Deployment:** Render (live web app).

**Skills:** Recommendation system design, scoring algorithm development, REST API design, frontend development, literature synthesis.

**Results:** The tool covers 25+ activities across 7 categories (Movement, Creative, Social, Rest, Learning, Meaning, Sensory), with each recommendation linked to a peer-reviewed mechanism and a specific, actionable tip. The web interface allows real-time filtering by mood, time, energy, and preferred category, returning a ranked menu in under one second.

### Pittsburgh Trauma Medical Center — ED Shift Analytics

**Code:** [pitt-ed-analytics](https://github.com/wchai0721/Projects/tree/main/pitt-ed-analytics)

**File(s):** [.twbx](https://public.tableau.com/shared/QP3QXGT9Q?:display_count=n&:origin=viz_share_link)

**Goal:** To model emergency department patient flow across a 15-hour trauma shift and surface operational insights around wait times, care bottlenecks, staff load, and disposition outcomes.

**Description:** This project simulates a realistic ED shift at a Level 1 trauma center, inspired by the TV series The Pitt. Using a synthetic dataset of 180 patients generated with Python and Faker, the project involved designing a relational schema across six tables, loading data into PostgreSQL, writing analytical SQL queries using window functions and CTEs, organizing transformations as dbt models with staging and mart layers, and visualizing findings in an interactive Tableau Public dashboard.

**Technology:** Python, Faker, PostgreSQL, dbt, Tableau Public.

**Skills:** Relational schema design, SQL window functions, CTEs, data modeling, dbt transformation layer, dashboard design.

**Results:** ESI 4 and 5 patients waited 40+ minutes on average for a provider while ESI 1 patients were seen in under 5 minutes. Imaging was identified as the single largest care bottleneck at approximately 88 minutes average. Attending load peaked mid-shift between hours 10 and 16, with Dr. Dana Evans carrying the highest sustained patient volume. ESI 1 and 2 patients were predominantly admitted to the ICU or deceased, while ESI 4 and 5 patients were mostly discharged or left without being seen.

### GreenTech Recycling Operations Dashboard

**File(s):** [.twbx](https://public.tableau.com/views/greentech-recycling/Inventory?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link) · [GreenTech Recycling Data (Excel)](https://github.com/wchai0721/Projects/blob/main/GreenTech_Recycling_Tableau_Data.xlsx)

**Data source:** Simulated operational data modeled from client ERP, time-tracking, and financial records.

**Goal:** To surface operational bottlenecks, labor inefficiencies, and financial performance gaps across an electronics recycling workflow, and to replace manual Excel-based reporting with a dynamic, decision-ready dashboard.

**Description:** This project was completed as part of a Carlson Consulting Enterprise (CCE) engagement through the University of Minnesota's Carlson Analytics Lab. Working directly with the client's CFO, the team mapped the full operational workflow from receiving through teardown and resale, identified key performance indicators across four process stages (Receiving, Sort, Testing/Repair, and Teardown), and designed a three-dashboard Tableau prototype to replace fragmented manual reporting. The project involved process mapping, stakeholder interviews, KPI prioritization, dashboard wireframing, and data pipeline planning across three source systems. The Tableau build used five structured data tables with inter-sheet relationships, calculated fields for fail rate, throughput, and budget variance, and global filter actions to enable cross-dashboard interactivity.

**Technology:** Tableau Public, Microsoft Excel.

**Skills:** Process mapping, KPI design, dashboard design, data modeling, stakeholder communication, Excel data pipeline structuring, Tableau relationships and calculated fields.

**Results:** Analysis revealed that Testing/Repair is the primary operational bottleneck, accounting for the highest labor hours across all four channels. The testing fail rate averaged 51.4%, indicating significant upstream sorting inefficiencies. Financial analysis showed that the client averaged a net loss of $51,616 annually since 2011, with a catastrophic outlier loss of $707,431 in 2019 (6x any other year), and that contributions and grants have been essential to keeping the organization net-positive in most years. The dashboard framework positions the client to shift from intuition-based to data-driven decision making ahead of their self-sustainability goal.

### iPSC Cell Line Bank – Product Pricing & Revenue Model

**File(s):** [XYZ University iPSC_CellBank_Pricing.xlsx](https://github.com/wchai0721/Projects/blob/main/XYZ%20University_iPSC_CellBank_Pricing.xlsx)

**Data source:** Cost estimates derived from published stem cell core pricing surveys and vendor catalogs (StemCell Technologies, Thermo Fisher Scientific, BioLife Solutions); reagent and labor rates benchmarked against WiCell and Cedars-Sinai iPSC Core published fee schedules

**Goal:** To develop a scenario-based pricing framework for a university-operated induced pluripotent stem cell (iPSC) bank, enabling cost-recovery planning, tiered access pricing, and multi-year revenue forecasting as the program scales toward a service core model.

**Description:** The model covers 10 proposed product and service lines spanning banked iPSC vials, custom reprogramming, characterization packages, exosome harvest services, and spinal cord assembloid differentiation. Cost assumptions include a labor rate of $45/hr, reagent and media costs of $95/vial sourced from StemCell Technologies catalog pricing, cryopreservation supply costs of $18/vial, liquid nitrogen storage at $12/vial/year, and a 20% overhead allocation. These inputs feed a global assumption layer that propagates automatically through all pricing calculations. Regional pricing tiers stratify customers from internal academic users to large pharmaceutical companies. A five-year scenario analysis models revenue and gross profit across conservative, base, optimistic, scale, and mature growth trajectories. A companion NPI tracker sheet manages the stage-gate launch pipeline for all 10 product lines, with milestone definitions, cross-functional ownership, and live budget tracking.

**Technology:** Microsoft Excel (dynamic formula modeling, conditional formatting, scenario analysis, tiered pricing dashboard).

**Skills:** Financial modeling, pricing strategy, scenario analysis, product launch planning, research core operations.

**Results:** At base-case assumptions (45% target gross margin), the bank projects approximately $370K in annual revenue across all service lines, with the conservative Year 1 scenario yielding roughly $185K. Biological and cell-based services — including assembloid differentiation and exosome harvest — represent high-margin opportunities with strong growth potential as preclinical interest in cell-based therapeutics continues to expand.

### iPSC Cell Line Bank – New Product Introduction (NPI) Launch Tracker

**File(s):** [XYZ University iPSC_CellBank_NPI.xlsx](https://github.com/wchai0721/Projects/blob/main/XYZ%20University_iPSC_CellBank_NPI.xlsx)

**Data source:** Stage-gate framework adapted from standard new product introduction methodology; milestone criteria informed by published academic core facility launch guidelines and FDA biological product development guidance
Goal: To provide a structured, cross-functional project management tool for tracking the phased launch of 10 new product and service lines within a university-operated iPSC cell line bank, from initial feasibility through full commercial scale.

**Description:** The tracker maps each product line across a four-phase stage-gate framework — Feasibility, Development, Pilot Launch, and Scale — with defined exit criteria, named approvers, and required documentation at each gate. For each of the 10 service lines, the tracker captures the assigned lead and cross-functional team (spanning research, IRB, biosafety, legal, finance, QA, and facilities), planned start and target launch dates, milestone gate definitions, live status badges, percent completion, and budget versus actual spend. A milestone gate definitions table codifies institutional sign-off requirements at each phase transition, including IRB pre-review, SOP validation, IP clearance through technology transfer, and export control compliance for international distribution. A budget dashboard auto-aggregates spend utilization, phase distribution, and average completion rate across the full product portfolio.

**Technology:** Microsoft Excel (dynamic formula modeling, conditional formatting, stage-gate dashboard).

**Skills:** Project management, stage-gate product development, cross-functional coordination, budget tracking, research core operations, academic technology commercialization.

**Results:** Across 10 planned service lines, the tracker identifies approximately $294K in total program budget, with early-stage products concentrated in Phases 1 and 2. Custom reprogramming and characterization services are furthest along at 55% and 70% complete respectively, representing the fastest path to revenue. Higher-complexity offerings — assembloid differentiation and international distribution — are staged to Phases 3 and 4 to allow supporting infrastructure (IP framework, export licensing, QA systems) to mature in parallel with scientific readiness.

## Education

**University of Minnesota — Carlson School of Management** Master of Business Administration — Medical Industry Leadership & Business Analytics (May 2023)

**University of Cincinnati — College of Medicine** Master of Science — Developmental Biology & Transfusion Medicine (May 2014)

**University of Minnesota — College of Biological Sciences** Bachelor of Science — Biochemistry (May 2012)

## Certificates

**[Programming for Everybody](https://coursera.org/share/c8fc2695991231056b55efb7a8f936c8)** (Coursera - University of Michigan)

**[SQL for Beginner Data Analysis](https://www.udemy.com/certificate/UC-70dcbf78-a39a-4d88-a8a4-804af89e38e6/)** (Udemy)

## Contact

- LinkedIn: [@wenchai](https://www.linkedin.com/in/wenchai/)
- Email: [wchai0721@gmail.com](mailto:wchai0721@gmail.com)
