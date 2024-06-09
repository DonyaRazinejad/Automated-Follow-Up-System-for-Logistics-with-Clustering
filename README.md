# Automated-Follow-Up-System-for-Logistics-with-Clustering
Automate Follow-Up System for the Logistics Department with the Help of Machine Learning , Capston Project.

This code is part of our team capstone project, where I contributed to the backend development. The follow-up system automates reminders for orders at strategic intervals, specifically at 50%, 75%, and one day before the due date. It utilizes K-Means clustering to analyze and categorize products and suppliers based on factors such as lead time, back-order days, and delivery cost.

Ranking System for Follow-Up
How the Ranking System Works:
Data Collection: The system collects historical data on product lead times, back-order days, and delivery costs, as well as supplier performance metrics such as delivery accuracy and fulfillment times.

Clustering: Using K-Means clustering, the system groups products and suppliers into distinct clusters based on the collected data. Each cluster represents a group of products or suppliers with similar characteristics.

Cluster Ranking:

Product Clusters: Products are ranked based on their lead times and back-order days. Products with longer lead times and higher back-order days receive a higher rank (indicating a higher likelihood of delay).
Supplier Clusters: Suppliers are ranked based on their historical delivery performance. Suppliers with a history of late deliveries receive a higher rank.
Cumulative Rank Calculation: For each order, the system calculates a cumulative rank by summing the rank of the product cluster and the rank of the supplier cluster. This cumulative rank provides a numerical indicator of the follow-up priority.

Follow-Up Decision Process:
High Priority Orders:

Criteria: Orders with high cumulative ranks (indicating high risk of delays).
Follow-Up Strategy: These orders receive multiple follow-ups—at 50% of the lead time, at 75% of the lead time, and one day before the due date.
Medium Priority Orders:

Criteria: Orders with medium cumulative ranks.
Follow-Up Strategy: These orders receive two follow-ups—at 75% of the lead time and one day before the due date.
Low Priority Orders:

Criteria: Orders with low cumulative ranks (indicating low risk of delays).
Follow-Up Strategy: These orders receive a single follow-up one day before the due date.
Benefits:
Proactive Management: By prioritizing orders based on the likelihood of delays, the system ensures timely communication and proactive issue management.
Resource Optimization: Follow-up efforts are focused where they are most needed, optimizing resource use and improving overall efficiency.
Improved Customer Satisfaction: Timely follow-ups help ensure orders are delivered on time, enhancing customer satisfaction and reliability.
By leveraging machine learning and clustering techniques, our follow-up system provides a structured and efficient approach to managing logistics, significantly reducing the incidence of late deliveries.
