# Zachary Shah
## Medical Supplier Dashboard

Wanting to familiarize myself with foundry and its workflow, I began thinking on some practical use cases. I personally didn't handle lots of spreadsheets and  documents on a daily basis, but I knew someone who did: my dad. He owns a private practice allergy company, and I recalled how every so often our fridge would fill up with new shipments of extracts before being taken to his office. Asking my dad on how he tracks his orders and when he decides to buy more, I learned that there was actually quite a lot of mechanics behind the scenes.

My dad is part of a group of practices, who agree to buy some products in bulk as medical suppliers offer discounts with larger orders. A friend of my dad, who works at a medical supplier, agreed to share with me their sales data for a specific grouping. The data was broken down by product type and account type. So thus a project began, to see how I could optimize this current system given only the information I had at hand.

![alt text](https://github.com/zachary-shah-27/Foundry-Medical-Supplies-Dashboard/blob/main/Shah_Pipeline_Builder.png "pipeline builder")

I started by smoothing the data in pipeline builder. I found many of the total sale counts were added incorrectly, so I went back and adjusted the columns. I separated the customer ID from the string names, and calculated percent changes over the past 2 years (and current YTD) to see which companies were buying more, and which were buying less. Similarly for the list of products: which ones were selling well and which ones were selling poorly.

![alt text](https://github.com/zachary-shah-27/Foundry-Medical-Supplies-Dashboard/blob/main/Shah_Sections_in_depth.png "section table")

To make the product category more readable, I used pipeline builder to filter keywords from the product names, and place them into common categories (called "Sections" in this table). This way, I could track the success of an entire product type and get a more accurate depiction of said product type's sales.

From the pipeline I created 3 data tables: The first, 'Account Data', represents individual customer accounts — each row contains a customer ID, full customer string, and a two-year percent change in purchases, which can be used to compare growth and churn risk across practices. The second dataset, 'Product Data', captures general product type (like "syringes" or "pollen"), the specific product name, and its two-year percent change. This lets me see which products or categories are performing well or declining. The third dataset, 'Deviation', lists the overall variability within each product type, containing the product section name and its standard deviation from the aggregate. Unusually high volatility may warrant closer inspection and offer potential "bundle" opportunities.

![alt text](https://github.com/zachary-shah-27/Foundry-Medical-Supplies-Dashboard/blob/main/Shah_whole_dashboard.png "whole dashboard")

Combining my tables into a linked ontology, this is the finished result of a potential usable dashboard. The core operation, from the perspective of the medical supplier, is to match volatile products to volatile customers; taking advantage of out-performing products and growing buyers, and holding on to customers at risk of churn. The left side identifies products and product types and their respective metrics, while the right side offers churn-risk buyers and growing buyers. You can match products to buyers and automatically send an email offer.

![alt text](https://github.com/zachary-shah-27/Foundry-Medical-Supplies-Dashboard/blob/main/Shah_Churn_companies.png "churn companies")

![alt text](https://github.com/zachary-shah-27/Foundry-Medical-Supplies-Dashboard/blob/main/Shah_leader_companies.png "leader companies")

Ideally, churn companies can be cut better individual deals in return for them buying more products. One way to prevent churn could be to offer a bundle of top performing products (which the customer wants) along with poor performing products at a further discounted price. For growing companies, we can target the poor selling products and ask if they would be willing incentivize the group of practices to buy at a discount.

![alt text](https://github.com/zachary-shah-27/Foundry-Medical-Supplies-Dashboard/blob/main/Shah_Under_watch.png "under watch")

Categories "under watch" are categories of high volatility: either moving up or down. These categories likely would benefit from some type of discount or bundle.
