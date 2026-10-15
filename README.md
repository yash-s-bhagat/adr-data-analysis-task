# adr-data-analysis-task

Adverse Drug Reaction (ADR) Data Analysis

1. Project Overview

This project analyzes healthcare data containing Adverse Drug Reaction (ADR) reports to identify patterns between suspected medicines, patient symptoms, and reported reactions. It uses Python libraries to clean, summarize, and visualize sample ADR data.

The project demonstrates a basic pharmacovigilance data analysis workflow, including reaction frequency analysis, suspected drug analysis, seriousness assessment, and reporting trends over time.

2. Project Objectives

- Analyze ADR reports containing patient and medication information.
- Identify commonly reported suspected drugs.
- Determine the frequency of different adverse reactions.
- Compare serious and non-serious ADR reports.
- Analyze ADR reporting trends over time.
- Explore patient age and reaction onset timelines.
- Generate charts and summary reports using Python.

3. Tools and Technologies

- Programming Language: Python
- Data Analysis: Pandas
- Data Visualization: Matplotlib
- Dataset Format: CSV
- Version Control: Git and GitHub

4. Project Structure

adr-data-analysis-task/
├── data/
│   └── adr_reports.csv
├── src/
│   └── analyze_adr_data.py
├── outputs/
│   ├── drug_report_counts.png
│   ├── reaction_counts.png
│   ├── seriousness_distribution.png
│   ├── monthly_reporting_trend.png
│   ├── drug_report_counts.csv
│   ├── reaction_counts.csv
│   ├── seriousness_summary.csv
│   ├── monthly_reports.csv
│   └── summary_metrics.csv
├── requirements.txt
└── README.md

5. Dataset Description

The dataset contains synthetic ADR reports with the following fields:

Field| Description
report_id| Unique ADR report identifier
age| Patient age
gender| Patient gender
suspected_drug| Medicine suspected of being associated with the reaction
reaction| Reported adverse reaction
onset_days| Days between medicine use and reported reaction
outcome| Reported outcome
serious| Whether the report is marked serious
report_date| Date of the report

Note: The dataset is synthetic and created for educational purposes. It does not contain real patient information.

6. Analysis Performed

A. Suspected Drug Analysis

Counts ADR reports associated with each suspected medicine to identify which medicines appear most frequently in the sample.

B. Adverse Reaction Analysis

Examines the frequency of reported reactions, such as rash, nausea, diarrhea, bleeding, and stomach pain.

C. Seriousness Analysis

Compares reports marked serious with those marked non-serious and calculates the percentage of serious reports in the sample.

D. Reporting Trend Analysis

Groups reports by month to visualize how the number of reports changes over time.

E. Summary Statistics

Calculates the total number of reports, number of suspected drugs, number of distinct reactions, mean patient age, mean onset time, and seriousness percentage.

7. Installation and Requirements

Install Python 3.9 or later.

Install the required libraries by running:

pip install -r requirements.txt

The "requirements.txt" file contains:

pandas>=2.0
matplotlib>=3.7

8. How to Run the Project

Open a terminal in the project directory and run:

python src/analyze_adr_data.py

The script processes the dataset, removes duplicate report IDs, creates summary CSV files, and generates visualization charts inside the "outputs/" folder.

9. Expected Outputs

The project generates the following charts:

- "drug_report_counts.png" — ADR report counts by suspected drug.
- "reaction_counts.png" — Frequency of reported reactions.
- "seriousness_distribution.png" — Distribution of serious and non-serious reports.
- "monthly_reporting_trend.png" — Monthly ADR reporting trend.

It also generates CSV summary files for drug counts, reaction counts, seriousness, monthly reports, and overall metrics.

10. Key Findings

The supplied sample dataset contains:

- 36 unique ADR reports.
- 6 unique suspected medicines.
- 9 distinct reported reaction types.
- 13 reports marked serious.
- 36.1% of reports marked serious.
- 49.9 years average patient age.
- 3.5 days average reported onset time.

These findings describe only the synthetic dataset and should not be interpreted as real-world drug safety statistics.

11. Limitations

- The dataset is synthetic and relatively small.
- The number of reports does not establish the actual risk associated with a medicine.
- A reported reaction does not prove that the suspected drug caused it.
- Real pharmacovigilance assessments require validated clinical information and appropriate medical and statistical review.

12. Conclusion

This project demonstrates how Python, Pandas, and Matplotlib can be used to analyze and visualize sample adverse drug reaction reports. The analysis helps organize suspected drug information, reported reactions, seriousness classifications, and reporting timelines into understandable charts and summary tables.

The project provides a foundation for learning healthcare data analysis and pharmacovigilance workflows.

13. Author

B.Pharmacy Graduate | Pharmacovigilance and Healthcare Data Analytics

14. Disclaimer

This project is intended for educational and internship purposes only. It is not intended for diagnosis, treatment decisions, regulatory decisions, or real-world drug safety conclusions.