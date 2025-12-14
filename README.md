# Why Do AI/ML Professionals Earn More?

## Project Overview
This project analyzes **why AI/ML professionals consistently earn higher salaries** compared to other software and data roles. Using data from the **Stack Overflow Developer Survey (2020–2024)**, the analysis investigates how experience, company scale, AI engagement, and sentiment toward AI influence compensation levels.

The project combines exploratory analysis with a **multiple linear regression (MLR)** model to identify statistically significant drivers of developer pay.

---

## Research Question
**Why do AI/ML professionals earn more than other technology roles?**

Key sub-questions:
- Do AI/ML roles consistently lead in pay across years?
- How do experience and organization size affect compensation?
- Does sentiment toward AI or fear of AI job displacement impact earnings?

---

## Data Source
- **Stack Overflow Developer Survey (2020–2024)**
- Focus on the **2024 dataset** (~65,000 respondents)
- Public, self-reported developer survey data

---

## Dataset & Variables

### Target Variable
- **AnnualComp**  
  Normalized annual compensation in USD

### Key Predictors
- **YearsCodeProNum** – Years of professional coding experience  
- **OrgSizeNum** – Organization size  
- **RoleGroup** – Software, Data, AI/ML, and hybrid roles  
- **UsesPython** – Python usage indicator  
- **RemoteWorkNum** – Remote work status  
- **AISentNum** – Sentiment toward AI  
- **AIThreatNum** – Perceived AI job threat  

---

## Methodology

### Data Preparation
1. Imported and merged survey data from 2020–2024
2. Cleaned and normalized compensation values
3. Engineered categorical groupings for developer roles
4. Encoded AI sentiment and AI threat perception variables

### Modeling Approach
- Built a **Multiple Linear Regression (MLR)** model
- Objective: identify key factors influencing developer compensation
- Evaluated coefficient direction, magnitude, and explanatory power

---

## Key Findings

### Salary Trends
- **AI/ML roles consistently lead in average compensation**
- Pay increases with:
  - Professional experience
  - Organization size
  - Remote work
  - Python usage

### AI Perception
- Developers with **positive engagement with AI** earn more
- **Fear of AI as a job threat is associated with lower pay**
- AI threat perception is generally low across respondents

### Model Performance
- The model explains approximately **25% of salary variation**
- Average prediction error: **± $39,000**
- Indicates compensation is influenced by additional unobserved factors (negotiation, geography, specialization, etc.)

---

## Conclusions
Higher salaries among AI/ML professionals are driven primarily by:
- Greater experience and technical specialization
- Employment at larger organizations
- Active engagement with AI tools and programming languages (especially Python)

Professionals who **embrace AI benefit economically**, while those who perceive AI as a threat tend to fall behind.

---

## Tools & Technologies
- **Python**
- **Pandas, NumPy** – Data cleaning and transformation
- **Matplotlib / Seaborn** – Visualization
- **Statsmodels / Scikit-learn** – Regression modeling

---

## Repository Structure
```text
├── data/                 # Raw and cleaned survey datasets
├── notebooks/            # Analysis and modeling notebooks
├── figures/              # Charts and visualizations
├── presentation/         # Final presentation slides
└── README.md
