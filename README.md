# Customer Service Satisfaction Analysis
The main objective of this story is to analyze the CSAT trends and patterns within an e-commerce dataset.

Link to my [CSAT Analyst](https://public.tableau.com/app/profile/chi.nguyen6580/viz/CustomerServiceSatisfactionAnalysis/CustomerServiceSatisfactionAnalysis)

## About Dataset

[eCommerce Customer Service Satisfaction](https://www.kaggle.com/datasets/ddosad/ecommerce-customer-service-satisfaction/data) dataset captures customer satisfaction scores for a one-month period at an e-commerce platform called Shopzilla (a pseudonym). It includes various features such as category and sub-category of interaction, customer remarks, survey response date, category, item price, agent details (name, supervisor, manager), and CSAT score etc.

This dataset contains 20 columns and 85,907 rows:

| Column                  | Description                                              |
| :---------------------- | :--------------------------------------------------------|
| Unique id	              | Unique identifier for each record                        |
| Channel name	          | Name of the customer service channel                     |
| Category	              | Category of the interaction                              |
| Sub-category	          | Sub-category of the interaction                          |               
| Customer Remarks	      | Feedback provided by the customer                        |
| Order id	              | Identifier for the order associated with the interaction |  
| Order date time	        | Date and time of the order                               |
| Issue reported at	      | Timestamp when the issue was reported                    |
| Issue responded	        | Timestamp when the issue was responded to                |
| Survey response date	  | Date of the customer survey response                     |
| Customer city	          | City of the customer                                     |
| Product category	      | Category of the product                                  |
| Item price	            | Price of the item                                        |
| Connected handling time	| Time taken to handle the interaction                     |
| Agent name	            | Name of the customer service agent                       |
| Supervisor	            | Name of the supervisor                                   |
| Manager	                | Name of the manager                                      |
| Tenure Bucket	          | Bucket categorizing agent tenure                         |
| Agent Shift	            | Shift timing of the agent                                |
| CSAT Score	            | Customer Satisfaction (CSAT) score                       |

## Summary
- No duplicate values found while lot of missing data
- Average CSAT score: 4.24
- Total surveys: 85,907 (satisfied: 70,836 - unsatisfied: 15,071)
- Agents: 1,371
- Managers: 6
- Supervisors: 40

## 01. Top performing Managers and Supervisors:

![Customer Service Satisfaction Analysis](https://github.com/chilinh428/CSAT-Analysis-Story/assets/165115957/35053a8b-97e7-4ff4-a3e5-244c861b0635)

- Explore the plots by clicking on the `Manager` to get into more details:

![Customer Service Satisfaction Analysis (1)](https://github.com/chilinh428/CSAT-Analysis-Story/assets/165115957/77fe97fe-9911-4a25-ad04-80dc3bfa627a)

## 02. CSAT distribution by Channel and Tenure Bucket:

![Customer Service Satisfaction Analysis (2)](https://github.com/chilinh428/CSAT-Analysis-Story/assets/165115957/594f16d4-b9fe-40a3-ac30-4cd387065ed0)

## 03. CSAT distribution by Category and Sub-category:

![Customer Service Satisfaction Analysis (3)](https://github.com/chilinh428/CSAT-Analysis-Story/assets/165115957/49c54aa8-1319-4ed4-ac59-662a0b6e1b0d)

- Pareto analysis identifies the few important factors that contribute most to a problem, allowing us to focus efforts where they'll have the greatest impact for improvement.
As above, we see that 80% of negative feedback originates from just 20% of categories.

- Explore the plots by clicking on the `Category` to get into more details:

![Customer Service Satisfaction Analysis (5)](https://github.com/chilinh428/CSAT-Analysis-Story/assets/165115957/332e2d9a-2deb-41e9-a767-bfa74717f946)

## 04. CSAT distribution by Response Time:

![Customer Service Satisfaction Analysis (4)](https://github.com/chilinh428/CSAT-Analysis-Story/assets/165115957/b60e70b9-da2f-46fb-96f5-b85d21791b45)
