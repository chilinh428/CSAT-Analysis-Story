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

<img width="836" alt="Screenshot 2024-04-05 at 11 43 44" src="https://github.com/chilinh428/CSAT-Analysis-Story/assets/165115957/e3a21929-d4ff-46b4-8cd2-515f5e796891">

- Explore the plots by clicking on the `Manager` to get into more details:

<img width="836" alt="Screenshot 2024-04-05 at 11 44 16" src="https://github.com/chilinh428/CSAT-Analysis-Story/assets/165115957/f138e82b-3190-4257-a36e-147506947b52">

## 02. CSAT distribution by Channel and Tenure Bucket:

<img width="836" alt="Screenshot 2024-04-05 at 12 47 58" src="https://github.com/chilinh428/CSAT-Analysis-Story/assets/165115957/a5fb088e-d3b4-495a-abd3-c42e83729005">

- Advisors with a tenure exceeding 90 days conducted the highest number of surveys, possibly due to a higher call volume. Despite their extensive tenure, their CSAT stands at 4.27, which could have been higher.

- Trainee advisors had the lowest CSAT score at 4.15, which is expected since they are new to the system.
## 03. CSAT distribution by Category and Sub-category:

<img width="836" alt="Screenshot 2024-04-05 at 11 45 11" src="https://github.com/chilinh428/CSAT-Analysis-Story/assets/165115957/732efd6f-a2fc-4eee-9336-5e19afa8049b">

- Pareto analysis identifies the few important factors that contribute most to a problem, allowing us to focus efforts where they'll have the greatest impact for improvement.
As above, we see that 80% of negative feedback originates from just 20% of categories.

- Explore the plots by clicking on the `Category` to get into more details:

<img width="836" alt="Screenshot 2024-04-05 at 11 45 37" src="https://github.com/chilinh428/CSAT-Analysis-Story/assets/165115957/1e2f2c2d-48e8-4cbb-883e-8fd31e69fe8f">

## 04. CSAT distribution by Response Time:

<img width="836" alt="Screenshot 2024-04-05 at 11 45 51" src="https://github.com/chilinh428/CSAT-Analysis-Story/assets/165115957/7b762ae0-9ce1-498e-8182-f5e2e13fae46">

- From the chart above, we can see that the average response time is longer on the night shift, even when the number of reports is low.

- It is very clear that response time has an impact on CSAT. Faster response times result in better CSAT, whereas longer response times tend to decrease CSAT.
