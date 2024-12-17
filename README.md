# FCA
# Family Dynamics Analysis in France Using FCA

## Project Description
This project applies **Formal Concept Analysis (FCA)** to analyze family dynamics in France. It identifies patterns in family structures, single-parent households, childbearing decisions, and naturalization trends across five regional zones using census data.

---
## Table of Contents
1. [Project Overview](#project-overview)
2. [Methodology](#methodology)
3. [Technologies Used](#technologies-used)
4. [Data Sources](#data-sources)
5. [Installation and Execution](#installation-and-execution)
6. [Results Summary](#results-summary)
7. [Limitations](#limitations)
8. [References](#references)

---
## Project Overview
The study examines:
- Family structure and cohabitation patterns.
- Characteristics of single-parent households.
- Factors influencing childbearing decisions.
- Trends in naturalization through marriage.

By employing **FCA**, the project extracts meaningful patterns and generates visual representations (concept lattices) to uncover relationships within census data.

---
## Methodology
1. **Problem Definition**: Analyze family-related variables to identify significant patterns.
2. **Data Preparation**:
   - Extracted a sample of 3 million rows per region from the national census dataset.
   - Features include marital status, nationality, household size, and professional status.
3. **Technical Implementation**:
   - Utilized Python libraries: `FCApy`, `caspailleur`, and `paspailleur`.
   - Data mining algorithms were used to identify stable and interesting patterns.
4. **Results Analysis**:
   - Generated concept lattices to visualize relationships among variables.
   - Measured pattern support and stability using Delta measures.

---
## Technologies Used
- **Programming Language**: Python
- **Libraries**:
   - FCApy (Formal Concept Analysis)
   - caspailleur (Pattern mining for binary data)
   - paspailleur (Pattern mining for complex data)
- **Hardware**: NVIDIA A100 GPU (PNY Server)

---
## Data Sources
- Data provided by **The National Institute of Statistics and Economic Studies (INSEE)**.
- Dataset: "Housing, individuals, activity, educational and occupational mobility, residential migration in 2016."
- Regional zones analyzed:
   - Zone A: Île-de-France
   - Zone B: Centre-Val de Loire, Bourgogne-Franche-Comté, Normandie, Hauts-de-France
   - Zone C: Grand Est, Pays de la Loire, Bretagne
   - Zone D: Nouvelle-Aquitaine, Occitanie
   - Zone E: Auvergne-Rhône-Alpes, Provence-Alpes-Côte d’Azur, Corse, Overseas regions

---
## Installation and Execution
### Prerequisites
- Python 3.8+
- Required libraries installed:
   ```bash
   pip install FCApy
   pip install caspailleur
   pip install paspailleur
   ```

### Steps to Run the Project
1. **Clone the Repository**:
   ```bash
   git clone <repo-link>
   cd <repo-directory>
   ```
2. **Prepare the Dataset**:
   - Place the dataset in the `data/` directory.
3. **Run the Analysis**:
   ```bash
   python main.py
   ```
4. **View Results**:
   - Outputs include pattern analysis, concept lattices, and stability measures.

---
## Results Summary
### Key Findings:
- **Family Structure**: Predominantly nuclear families with 2-5 members; emerging trends in shared accommodations (Zone C).
- **Single-Parent Households**: Common across all zones, often with extended family support (Zones C, D, E).
- **Childbearing Decisions**: Influenced by marital status and employment stability; higher education may delay family formation.
- **Naturalization Trends**: Significant among Portuguese, Algerian, Moroccan, and Italian populations, driven by historical and geographical ties.

### Visual Outputs:
- Concept lattices for each zone (Appendix).
- Scatter plots showing pattern support and Delta measures.

---
## Limitations
1. **Resource Constraints**: High memory requirements (100GB RAM) limited dataset size.
2. **Algorithmic Limitations**: Extracted patterns were less precise due to implementation constraints.
3. **Dataset Scope**: Excluded marital subcategories (e.g., divorced, widowed) that could provide deeper insights.

---
## References
1. INSEE: French National Census Data.
2. Buzmakov et al. (2023), *Data Complexity: An FCA-Based Approach*.
3. Uta Priss (2023), *FCA Software Tools*. 
4. Kuznetsov & Obiedkov (2002), *Formal Concept Analysis Algorithms*.
5. GitHub Libraries: FCApy, caspailleur, paspailleur.

