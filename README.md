# Monte Carlo Simulation based on Zohran Mamdani Policies

This project aims to answer the question "Q. Can Zohran Mamdani Afford His Policies?".
This project is a Monte Carlo Simulation Using NYC's FY 2025 Budget

The central question is 
"Can Zohran Mamdani afford his proposed policies using a Monte Carlo budget simulation?"

The analysis uses real New York City financial data from the FY 2025 Annual Comprehensive Financial Report (ACFR) and simulates the fiscal impact of several policy proposals, including free buses, a grocery stipend, rent freeze support, administrative overhead, and rare housing-related payouts.

This repository evaluates whether these policies are fiscally feasible when added to NYC's actual 2025 financial structure.



## Inspiration

This project was inspired by the Kaggle Notebook:

[NYC Policy Monte Carlo Simulation](https://www.kaggle.com/code/kmaniv/nyc-policy-monte-carlo-simulation/notebook)


This project builds upon the work already established by the kaggle notebook by using audited financial data from New York City's FY 2025 ACFR.

A special thank you to the orignial author "kmaniv" on kaggle for the inspiration for this project.

## Data Source

There 2 main sources of data:
1. The Baseline Values
2. Proposed Policy Values from Mamdani


#### 1.  Baseline Values

All baseline FY 2025 financial values used in this model are taken from:

The City of New York  
Annual Comprehensive Financial Report  
Of the Comptroller  
For the Fiscal Years Ended June 30, 2025 and 2024

Link to the data source 
[ACFR 2025 website](https://comptroller.nyc.gov/reports/annual-comprehensive-financial-reports/)
[ACFR 2025 pdf](https://comptroller.nyc.gov/wp-content/uploads/documents/113208_Whitebook_bookmarked.pdf)


Values were manually extracted from:
- Page 42 of the PDF  
- Corresponding to page 76 out of 535 in the document

These values include:
- Governmental Activities expenses by function  
- Governmental Activities program revenues  
- Governmental Activities general revenues  

#### 2.  Proposed Policy Values Inspired by Mamdani

The policy cost estimates used in this repository are modeled assumptions inspired by the public descriptions of Zohran Mamdani’s proposals.

No numerical values were taken from his official policy documents.
No actual cost estimates are published on his platform for these programs.

Because this repository is inspired by the original [Kaggle notebook](https://www.kaggle.com/code/kmaniv/nyc-policy-monte-carlo-simulation/notebook), most numerical policy values were derived from or adapted from that work.

## Work done in the reporsiory

- Builds a fiscal baseline using official NYC governmental activities data  
- Adds Monte Carlo uncertainty to both revenues and expenses  
- Models the costs of Mamdani's proposed policies  
- Includes uncertainty about policy implementation  
- Implements a rare high-cost housing event to reflect landlord compensation risk  
- Models a progressive tax package designed to fund the policies  
- Computes:  
  - Mean surplus or deficit  
  - 5th and 95th percentile outcomes  
  - Probability that NYC finishes the year with a surplus  
- Visualizes the fiscal distribution under baseline and policy scenarios



## Requirements

This code was run on a python environment runing Python 3.10.0

The libraries used for this project are given below

- NumPy  
- Pandas  
- Matplotlib  
- Jupyter Notebook  

## Install dependencies

```bash
pip install -r requirements.txt
```

## Acknowledgments

- Kaggle user kmaniv for the original Monte Carlo concept  
- NYC Comptroller's Office for providing the ACFR  
- Publicly available policy documents associated with Zohran Mamdani

## License

MIT License.
