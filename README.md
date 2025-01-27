# eCommerce-Transactions-Dataset
eCommerce Transactions dataset consisting of three files:

Customers.csv:
https://drive.google.com/file/d/1bu_--mo79VdUG9oin4ybfFGRUSXAe-WE/view?usp=sharing

Products.csv :
https://drive.google.com/file/d/1IKuDizVapw-hyktwfpoAoaGtHtTNHfd0/view?usp=sharing

Transactions.csv :
https://drive.google.com/file/d/1saEqdbBB-vuk2hxoAf4TzDEsykdKlzbF/view?usp=sharing

Files Description:
1. Customers.csv
○ CustomerID: Unique identifier for each customer.
○ CustomerName: Name of the customer.
○ Region: Continent where the customer resides.
○ SignupDate: Date when the customer signed up.

2. Products.csv
○ ProductID: Unique identifier for each product.
○ ProductName: Name of the product.
○ Category: Product category.
○ Price: Product price in USD.

3. Transactions.csv
○ TransactionID: Unique identifier for each transaction.
○ CustomerID: ID of the customer who made the transaction.
○ ProductID: ID of the product sold.
○ TransactionDate: Date of the transaction.
○ Quantity: Quantity of the product purchased.
○ TotalValue: Total value of the transaction.
○ Price: Price of the product sold.

**Task 1: Exploratory Data Analysis (EDA) and Business Insights**
1. Perform a EDA on the provided dataset.
2. Derived 5 business insights from the EDA.

Deliverables:
● A Python script containing with EDA code.
● A PDF report with business insights.


**Task 2: Lookalike Model**
Build a Lookalike Model that takes a user's information as input and recommends 3 similar customers based on their profile and transaction history. 
The model should:
● Use both customer and product information.
● Assign a similarity score to each recommended customer.

Deliverables:
● Give the top 3 lookalikes with there similarity scores for the first 20 customers (CustomerID: C0001 - C0020) in Customers.csv. Form an “Lookalike.csv” 
which has just one map: Map<cust_id, List<cust_id, score>>

Evaluation Criteria:
● Model accuracy and logic.
● Quality of recommendations and similarity scores.


**Task 3: Customer Segmentation / Clustering**
Perform customer segmentation using clustering techniques. Use both profile information (from Customers.csv) and transaction information (from Transactions.csv).
● clustering algorithm and any number of clusters in between(2 and 10)
● Visualise your clusters using relevant plots.

Deliverables:
● A report on your clustering results, including:
○ The number of clusters formed.
○ DB Index value.
○ Other relevant clustering metrics.
● A Python script containing your clustering code.

Evaluation Criteria:
● Clustering logic and metrics.
● Visual representation of clusters.

**Clustering Approach**
We used three clustering techniques to segment customers:
1.	K-Means Clustering: This algorithm divides data into a fixed number of clusters, where each customer belongs to the closest cluster center. We tried different numbers of clusters (from 2 to 10) to identify the best fit.
2.	DBSCAN (Density-Based Spatial Clustering of Applications with Noise): DBSCAN groups points that are close to each other, identifying clusters based on density. It also marks outliers as noise.

Visualized the clustering results using Principal Component Analysis (PCA), which reduces the data to two dimensions. This helped us plot and visually inspect how well the clusters were separated. Each customer was assigned a color based on their cluster, making it easy to see the groupings.
