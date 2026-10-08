# UTD ASA Predictive Modeling Case Competition 2026

## Overview

This repository contains my team's work for the **2026 UT Dallas Actuarial Student Association (UTD ASA) Predictive Modeling Case Competition**, based on the CAS Predictive Modeling Case Study.

The case placed participants in the role of the pricing function for **Alpha Beta Gamma (ABG) Insurance**, a regional personal lines insurer seeking to expand its presence in the renters insurance market.

The objective was to develop a predictive pricing strategy for ABG's dormitory insurance product using policyholder claim history, underwriting information, and student and dormitory characteristics.

## Business Problem

ABG Insurance historically charged every dormitory insurance customer the same premium. With additional policy and claims data now available, the company wanted to develop a more statistically informed pricing approach.

Our task was to develop a predictive modeling framework that could:

- Segment policyholders according to risk.
- Estimate expected insurance losses.
- Develop appropriate pricing for individual policyholders.
- Incorporate existing underwriting tiers.
- Consider expenses and profitability.
- Address differences between new and renewal business.
- Provide an implementation strategy for management.

The final recommendations were designed for presentation to ABG's CEO.

## Data

The competition dataset contains **10,000 policyholders with varying degrees of risk**.

Available information includes:

- Claim history
- Existing underwriting tiers
- Student characteristics
- Dormitory characteristics
- Distance to campus
- Academic and other policyholder information
- Coverage-specific claim information

The analysis considers four coverages included in ABG's dormitory insurance product:

1. **Personal Property**
2. **Additional Living Expense**
3. **Liability**
4. **Guest Medical**

## Analytical Approach

The project follows an end-to-end actuarial predictive modeling and pricing workflow.

### 1. Data Preparation & Exploratory Analysis

The data was reviewed for quality issues, duplicate records, missing information, unusual observations, and relationships between policyholder characteristics and insurance losses.

Exploratory analysis was used to investigate claim frequency and severity across different coverage types and risk characteristics.

### 2. Claim Frequency Modeling

Predictive models were developed to estimate claim frequency/risk for each coverage.

Model performance was assessed using holdout validation and diagnostic measures including:

- ROC curves
- Precision-recall curves
- Calibration analysis
- Lift analysis
- Model comparison metrics

### 3. Claim Severity Modeling

Separate severity models were developed to estimate the expected cost of claims.

Actual-versus-predicted diagnostics and validation results were used to evaluate model performance.

### 4. Risk Segmentation

Predictive results were translated into practical risk segments and incorporated into ABG's existing underwriting structure:

- Preferred
- Standard
- Non-Standard

Additional rating factors were used to further differentiate risk within the underwriting tiers.

### 5. Pricing Framework

Frequency and severity estimates were combined to develop expected loss estimates and coverage-level pricing.

The analysis then developed:

- Coverage base rates
- Risk-tier pricing
- Segment relativities
- Policyholder-level premiums
- Pricing reconciliation
- New versus renewal pricing considerations

### 6. Business Strategy

The technical results were translated into business recommendations addressing:

- Pricing implementation
- Expense considerations
- New versus renewal customers
- Profitability
- Risk monitoring
- Model monitoring and calibration
- Multi-year business strategy

## Repository Structure

```text
UTD-ASA-Case-Competition-2026/
│
├── ABG_Predictive_Pricing_Workbook.ipynb
│   └── Main predictive modeling and pricing analysis
│
├── ABG Insurance Predictive Pricing Strategy (3).pdf
│   └── Final executive presentation
│
├── abg_final_outputs/
│   ├── Model comparison results
│   ├── Frequency and severity validation
│   ├── Calibration diagnostics
│   ├── ROC and precision-recall plots
│   ├── Risk-tier analysis
│   ├── Segment relativities
│   ├── Coverage-level pricing
│   ├── Policyholder-level premiums
│   ├── Pricing reconciliation
│   └── Pro forma business projections
│
└── README.md


## Competition Deliverables

The competition required teams to combine actuarial modeling with business judgment and communicate their recommendations in a concise executive presentation.

The principal areas of evaluation included:

- Presentation skills
- Technical analysis
- Appropriate use of analytical tools
- Business knowledge

Our final deliverables included the predictive modeling analysis, pricing framework, business recommendations, and CEO-oriented presentation.

## Skills Demonstrated

- Actuarial pricing
- Predictive modeling
- Claim frequency modeling
- Claim severity modeling
- Model validation
- Risk segmentation
- Insurance pricing
- Data cleaning and exploratory analysis
- Business strategy
- Data visualization
- Python
- Jupyter Notebook
- Executive communication

## Author

**David Nana Yaw Owusu Bosompem**

BSc Actuarial Science  
SOA Exam P & FM

**Interests:** Actuarial Science | Insurance Analytics | Predictive Modeling | Statistics
