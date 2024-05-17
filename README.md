# Customer Churn Analysis with Python
### Uncovering Insights into Customer Cancellations

This repository contains a Python project focused on analyzing customer churn for a company with a large client base (800,000+). Faced with a high rate of inactive customers who canceled their service, the company seeks to understand the driving factors behind these cancellations and develop strategies to mitigate churn.

## Project Overview

This data analysis project was part of the "Python Journey" crash course offered by Hashtag. It leverages the power of Python libraries like Pandas and Plotly to extract valuable insights from customer data and provide actionable recommendations.

## Dataset

The project utilizes a dataset (``cancelamentos.csv``) containing customer information and a binary indicator of whether they canceled the service. The dataset includes features such as:

- `idade`: Age of the client
- `sexo`: Sex of the client
- ``tempo_como_cliente``: How long the client has been with the company (in months)
- ``frequencia_uso``: Client's frequency of use per month
- ``ligacoes_callcenter``: Number of calls the client made to the call center
- ``dias_atraso``: Number of days bills are overdue
- ``assinatura``: Type of subscription the client has (e.g., monthly, annual)
- ``duracao_contrato``: Duration of the client's contract
- ``total_gasto``: Total amount the client spent on services
- ``meses_ultima_interacao``: Time since the client's last interaction with the company (in months)
- ``cancelou``: Whether the client canceled (1) or not (0)

**Note:** The data in ```cancelamentos.csv``` is fictional and used for academic purposes.

## Analysis and Key Findings

The project follows a systematic approach:

1. **Data Loading and Exploration:** The data is loaded using Pandas, and its structure is examined for missing values and data type consistency.
2. **Data Cleaning:** Irrelevant columns and rows with missing values are removed to prepare the data for analysis.
3. **Cancellation Rate Analysis:** The overall cancellation rate is calculated to establish a baseline understanding of the churn problem.
4. **Feature Analysis:** The relationship between each customer feature and the cancellation outcome is investigated using:
    - *Grouped averages:* Calculate the average cancellation rate for each value of a feature (e.g., cancellation rate for clients with monthly vs. annual subscriptions).
    - *Histograms:* Visualize the distribution of each feature, separated by cancellation status, to identify patterns and potential cancellation drivers.
5. **Actionable Insights:** Based on the analysis, several key insights are identified:
    - Clients with monthly contracts have a significantly higher cancellation rate.
    - Clients who contact the call center more than four times are more likely to cancel.
    - Clients with bill payment delays of more than 20 days consistently cancel.
    - Clients with low total spending are prone to cancellation.
6. **Recommendations:** The project proposes actionable strategies to address these findings:
    - Offer discounts for annual and quarterly subscriptions to incentivize longer-term commitments.
    - Implement proactive customer support measures to address issues before they escalate to multiple calls to the call center.
    - Develop strategies for early intervention and payment assistance for clients experiencing payment delays.
    - Explore opportunities to expand service offerings and upsell to increase customer engagement and spending.

## Impact

By implementing these recommendations, the project demonstrates a significant reduction in the cancellation rate, decreasing from 56.7% to 9%.

## Libraries

- ``pandas``: For data manipulation and analysis.
- ``plotly``: For creating interactive visualizations.

## How to Explore the Project

1. Clone the repository to your local machine.
```
git clone https://github.com/vzucchetti/churn-analysis.git
```
2. Install the necessary libraries using
```
pip install pandas plotly.
```
3. Open and run the Jupyter notebook (``main.ipynb``) to walk through the analysis steps, view the visualizations, and explore the findings.

## Conclusion
This data analysis project showcases the capability to extract meaningful insights from customer data, enabling businesses to understand and address the challenge of customer churn effectively. By identifying key drivers of cancellation and developing data-driven strategies, companies can significantly improve customer retention and overall business performance.
