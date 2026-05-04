# Wen Chai - Data Analyst Portfolio
## About

Hi, I'm Wen! I’m a neuroscientist and product manager with a strong analytical background in stem cell biology, neuroscience, and translational research. I’m currently expanding my skills in data analytics and data science, with the goal of applying my scientific training, problem-solving mindset, and technical curiosity to uncover meaningful insights from complex datasets.

Throughout my research and professional experience, I have developed a strong foundation in experimental design, data interpretation, statistical thinking, scientific communication, and project management. I have worked with complex biological data, managed multi-step research workflows, analyzed experimental outcomes, and translated technical findings into clear reports, presentations, and strategic recommendations.

Beyond my professional work, I enjoy learning new data analysis tools, building practical systems in Notion, exploring creative ways to visualize information, and continuously improving my technical skills. I’m especially interested in the intersection of science, data, business, and storytelling.

My CV is available as a PDF.

This repository showcases my skills, projects, and ongoing progress in Data Analytics and Data Science.

## Table of Contents

- [About](#about)
- [Projects](#projects)
  - Python + SQL
    - [SCI Clinical Trial Landscape Analysis](https://github.com/wchai0721/Data-Analysis-Portfolio/blob/main/README.md#spinal-cord-injury-clinical-trial-landscape-analysis)
    - [Oncology In Vitro Clinical Trial Landscape Analysis](https://github.com/wchai0721/Data-Analysis-Portfolio/blob/main/README.md#oncology-in-vitro-clinical-trial-landscape-analysis)
  - Python
    - [Dopamine Menu Generator](https://github.com/wchai0721/Projects/blob/main/dopamine-menu/README.md)
  - SQL
  - Excel
  - Tableau
    - GreenTech Recycling Operations Dashboard
  - Power BI
  - Notion
  - R
  - Data cleaning
  - Data visualization
  - Statistical analysis
- [Education](#education)
- [Certificates](#certificates)
- [Contact](#contact)

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

**Code:** [dopamine-menu/](https://github.com/wchai0721/Projects/tree/main/dopamine-menu) · [README](https://github.com/wchai0721/Projects/blob/main/dopamine-menu/README.md)

**Data source:** Primary literature (positive psychology research, 2015–2023)

**Goal:** To generate personalized, evidence-backed restorative activity recommendations based on a user's current mood, available time, and energy level.

**Description:** The project built a two-interface Python tool — a CLI and a Flask web app — that scores and ranks restorative activities using a custom recommendation engine. Each activity in the database is grounded in positive psychology research (Seligman, Csikszentmihalyi, Fredrickson, Pennebaker, and others) and tagged with psychological mechanism, mood affinities, energy requirements, and a concrete behavioral tip. The scoring engine applies weighted bonuses for mood match, energy alignment, and time fit, with hard filters that remove incompatible activities before ranking.

**Technology:** Python, Flask, HTML/CSS/JavaScript.

**Skills:** Recommendation system design, scoring algorithm development, REST API design, frontend development, literature synthesis.

**Results:** The tool covers 25+ activities across 7 categories (Movement, Creative, Social, Rest, Learning, Meaning, Sensory), with each recommendation linked to a peer-reviewed mechanism and a specific, actionable tip. The web interface allows real-time filtering by mood, time, energy, and preferred category, returning a ranked menu in under one second.

### GreenTech Recycling Operations Dashboard

**Code:** not applicable (Tableau workbook — .twbx)

**Data source:** Simulated operational data modeled from client ERP, time-tracking, and financial records.

**Goal:** To surface operational bottlenecks, labor inefficiencies, and financial performance gaps across an electronics recycling workflow, and to replace manual Excel-based reporting with a dynamic, decision-ready dashboard.

**Description:** This project was completed as part of a Carlson Consulting Enterprise (CCE) engagement through the University of Minnesota's Carlson Analytics Lab. Working directly with the client's CFO, the team mapped the full operational workflow from receiving through teardown and resale, identified key performance indicators across four process stages (Receiving, Sort, Testing/Repair, and Teardown), and designed a three-dashboard Tableau prototype to replace fragmented manual reporting. The project involved process mapping, stakeholder interviews, KPI prioritization, dashboard wireframing, and data pipeline planning across three source systems. The Tableau build used five structured data tables with inter-sheet relationships, calculated fields for fail rate, throughput, and budget variance, and global filter actions to enable cross-dashboard interactivity.

**Technology:** Tableau Desktop, Microsoft Excel, openpyxl.

**Skills:** Process mapping, KPI design, dashboard design, data modeling, stakeholder communication, Excel data pipeline structuring, Tableau relationships and calculated fields.

**Results:** Analysis revealed that Testing/Repair is the primary operational bottleneck, accounting for the highest labor hours across all four channels. The testing fail rate averaged 51.4%, indicating significant upstream sorting inefficiencies. Financial analysis showed that the client averaged a net loss of $51,616 annually since 2011, with a catastrophic outlier loss of $707,431 in 2019 (6x any other year), and that contributions and grants have been essential to keeping the organization net-positive in most years. The dashboard framework positions the client to shift from intuition-based to data-driven decision making ahead of their self-sustainability goal.

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
