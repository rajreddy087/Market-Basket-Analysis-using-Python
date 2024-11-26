# Market Basket Analysis using Python
Market Basket Analysis using the Apriori algorithm to identify product associations.


### Overview
This project performs **Market Basket Analysis** using the **Apriori algorithm** to uncover associations between items in a retail dataset. By finding frequent itemsets and generating association rules, this analysis helps in understanding product relationships, which can be used for product bundling, recommendations, and inventory management.

### Key Features
- **Data Exploration**: Analyze the dataset and visualize the top purchased items.
- **Apriori Algorithm**: Apply the Apriori algorithm to generate frequent itemsets and association rules.
- **Association Metrics**: Evaluate the quality of the rules using **Support**, **Confidence**, and **Lift** metrics.

### Libraries Used
- `pandas`: Data manipulation and analysis.
- `matplotlib`, `seaborn`: Data visualization.
- `mlxtend`: Frequent pattern mining and association rule generation.
- `warnings`: To suppress deprecation warnings during execution.

### Dataset
The dataset contains transactions from a grocery store, with each row representing a product purchased by a customer. The goal is to analyze these transactions to find which items are frequently bought together.

### Steps Involved
1. **Data Loading**: The dataset is loaded using `pandas.read_csv()`.
2. **Data Preprocessing**: 
   - Group items purchased by each customer and create a "basket" format with binary values (1 if the item is purchased, 0 otherwise).
   - The dataset is processed to include the `Quantity` of each product purchased.
3. **Applying Apriori**: 
   - Use the Apriori algorithm to find frequent itemsets with a minimum support threshold.
   - Generate association rules from the frequent itemsets using **lift** as the metric.
4. **Filtering Rules**: 
   - Filter the generated rules using **Confidence** and **Lift** to retain the most useful associations.

### Insights from the Project:
**Frequent Itemsets:** Certain products are frequently purchased together, showing strong associations.

**Product Bundling Opportunities:** The analysis can suggest potential product bundles or promotional offers based on strong association rules.

**Customer Behavior:** By understanding which items tend to be bought together, businesses can optimize their inventory and marketing strategies.
