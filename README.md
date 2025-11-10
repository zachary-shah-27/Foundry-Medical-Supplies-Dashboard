# Zachary Shah
## Medical Supplier Dashboard

Wanting to familiarize myself with foundry and its workflow, I began thinking on some practical use cases. I personally didn't handle lots of spreadsheets and  documents on a daily basis, but I knew someone who did: my dad. He owns a private practice allergy company, and I recalled how every so often our fridge would fill up with new shipments of extracts before being taken to his office. Asking my dad on how he tracks his orders and when he decides to buy more, I learned that there was actually quite a lot of mechanics behind the scenes.

My dad is part of a group of practices, who agree to buy some products in bulk as medical suppliers offer discounts with larger orders. A friend of my dad, who works at a medical supplier, agreed to share with me their sales data for a specific grouping. The data was broken down by product type and account type. So thus a project began, to see how I could optimize this current system given only the information I had at hand.

![alt text](https://github.com/zachary-shah-27/Foundry-Medical-Supplies-Dashboard/blob/main/Shah_Pipeline_Builder.png "pipeline builder")

I started by smoothing the data in pipeline builder. I found many of the total sale counts were added incorrectly, so I went back and adjusted the columns. I separated the customer ID from the string names, and calculated percent changes over the past 2 years (and current YTD) to see which companies were buying more, and which were buying less. Similarly for the list of products: which ones were selling well and which ones were selling poorly.

![alt text](https://github.com/zachary-shah-27/Foundry-Medical-Supplies-Dashboard/blob/main/Shah_Sections_in_depth.png "section table")

To make the product category more readable, I used pipeline builder to filter keywords from the product names, and place them into common categories (called "section" in this table). This way, I could track the success of an entire product type and get a more accurate depiction of said product type's sales. 

![alt text](https://github.com/zachary-shah-27/Foundry-Medical-Supplies-Dashboard/blob/main/Shah_whole_dashboard.png "whole dashboard")



![alt text](https://github.com/zachary-shah-27/Foundry-Medical-Supplies-Dashboard/blob/main/Shah_leader_companies.png "leader companies")

![alt text](https://github.com/zachary-shah-27/Foundry-Medical-Supplies-Dashboard/blob/main/Shah_Churn_companies.png "churn companies")



![alt text](https://github.com/zachary-shah-27/Foundry-Medical-Supplies-Dashboard/blob/main/Shah_Under_watch.png "under watch")
