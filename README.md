# FUTURE_DS_02
# Customer Support Ticket Analysis

**Project Description:**
An end-to-end Python analysis of 8,500+ customer support tickets, revealing top issues, resolution time trends, and actionable recommendations to optimize support efficiency and improve customer satisfaction.

## Overview
In this project, we analyze customer support tickets to identify recurring issues, understand how ticket priority impacts resolution times, and surface actionable insights. The goal is to automate common responses, allocate resources effectively, and build a proactive support knowledge base.

## Repository Structure
```
customer-support-analysis/   
├── data/                     # Raw and cleaned datasets (CSV files)
├── notebooks/                # Jupyter notebooks with analysis steps
│   ├── 01-data-cleaning.ipynb
│   ├── 02-exploratory-analysis.ipynb
│   └── 03-visualizations.ipynb
├── src/                      # Python modules and helper scripts
│   ├── preprocess.py
│   ├── analysis.py
│   └── visualization.py
├── outputs/                  # Generated charts and word clouds (PNG)
├── README.md                 # Project README (this file)
└── requirements.txt          # Python dependencies
```

## Getting Started

### Prerequisites
- Python 3.8+ installed
- pip package manager

## Data Description
The `data/` folder contains two CSV files:
- `customer_support_tickets.csv`: Raw ticket-level data including descriptions, priorities, timestamps, and satisfaction ratings.
- `cleaned_tickets.csv`: Preprocessed dataset with tokens, resolved timestamps, and computed response/ resolution hours.

## Analysis Workflow
1. **Data Cleaning** (`notebooks/01-data-cleaning.ipynb`): Handle missing values, convert timestamp columns, preprocess text fields.
2. **Exploratory Analysis** (`notebooks/02-exploratory-analysis.ipynb`): Generate frequency counts, priority and type distributions.
3. **Visualizations** (`notebooks/03-visualizations.ipynb`): Create bar charts, histograms, word clouds, and boxplots.
4. **Scripts** (`src/`): Reusable functions for preprocessing, analysis, and plotting.

## Key Findings
- **Frequent Issues**: Top repeated problems include login errors, payment failures, and connectivity issues.
- **Priority Impact**: Critical tickets average ~7.15 hours to resolve; High and Low priorities average ~8 hours.
- **Ticket Volume**: Technical issues comprise ~60% of total tickets.
- **Customer Satisfaction**: Lower satisfaction ratings correlate with longer resolution times.

## Recommendations
- **Automate**: Implement chatbots / templated replies for top 5 issue categories.
- **Resource Allocation**: Dedicate more agents to Critical tickets to hit sub-6hr SLA.
- **Knowledge Base**: Build an FAQ portal addressing common technical and billing queries.
- **Continuous Monitoring**: Schedule weekly dashboards to track resolution metrics and satisfaction trends.



