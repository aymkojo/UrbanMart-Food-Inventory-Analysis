# UrbanMart-Food-Inventory-Analysis
this repo contains my final project from my virtual Data and Business Analytics Training Program for Tertiary Students offered by OQD.


![image](https://github.com/aymkojo/UrbanMart-Food-Inventory-Analysis/assets/88543602/1db59af3-0e9f-4f6c-809d-964f9a538300)


UrbanMart Food Inventory Analysis 
Business Problem Statement: 
 
UrbanMart, a rapidly growing grocery retailer, is seeking to optimize its profitability by implementing an effective pricing strategy for its diverse product range. Currently, the company faces challenges in managing the price points of its items to ensure they are both competitive and profitable, considering factors such as the cost of procurement, expected revenue, and markup profit.  
Moreover, with the perishable nature of many of its products, UrbanMart must also navigate the complexity of product expiry dates, which can significantly impact both inventory management and sales. 
By leveraging the available dataset, which includes details on item category, purchase price, purchase date, quantity, expiry date, item status, and unit price of items, UrbanMart aims to derive actionable insights that can guide its pricing and inventory management strategies. 
The company needs a data-driven solution that can provide insights into: 
1.	How to set selling prices that cover procurement costs, other operational costs, and deliver a reasonable profit margin. 
2.	How to manage inventory to minimize losses from near-expiry or expired items. 
3.	How to balance expected revenue with expected cost to ensure a positive profit margin. 
The ultimate goal is to enhance profitability while maintaining competitive pricing and ensuring customer satisfaction by offering fresh, high-quality products. 
Dataset Information 
DatasetName: UMFSData 
The dataset has the following columns: 
1.	ItemID: Unique identifier for each item. 
2.	ItemCategory: The category to which an item belongs, such as Dairy, Poultry, Bakery, etc. 
3.	ItemName: The name of the item. 
4.	PurchasePrice The amount of money paid by a buyer to acquire a product, service, or asset. 
5.	PurchaseDate: the date the item was purchased or added to the stock. 
6.	InitialQuantity: The initial quantity of the item when it was first stocked. 
7.	UnitCost: The unit cost refers to the cost of a single item or unit of measurement.  
8.	CurrentQuantity: The current quantity of the item in stock. 
9.	ExpiryDate: The date when the item will expire. 
10.	DaystoExpiry: The number of days left until the item expires. 
11.	ItemStatus: The current status of the item, e.g., whether it's still good to consume or expired. 
 
 
 
 
 
 
NB:  
❖	Purchase Price 
The purchase price is the amount of money paid by a buyer to acquire a product, service, or asset.   
 
❖	Unit Cost 
•	The unit cost refers to the cost of a single item or unit of measurement.  
•	The Unit Cost = Unit Purchase Price plus the Operational Cost  
❖	MarkupProfit: the amount by which the cost of a good is increased in order to get to the final selling price. 
•	It is the difference between the selling price of a good or service and its cost. It is expressed as a percentage above the cost. In other words, it is the premium over the total cost of the good or service that provides the seller with a profit. 
  
❖	SellingPrice: The price at which the item is being sold. 
❖	An Expiry Date, also known as an expiration date, is the date after which something should no longer be used, either by operation of law or by exceeding the anticipated shelf life for perishable goods.  
 
 
 
 
 
 
 
 
Part 1: Inventory Metrics 
Important Metrics and KPIs to find include the ff: 
•	PurchasePricePerItem 
•	ExpectedCostPerProductQuantity 
•	TotalExpectedCost  
•	Profitability Metrics 
▪	UnitCostPricePerProduct: Hint: Increase the UnitCost by 20% 
▪	UnitMarkupProfit 
▪	MarkupProfitPerProductQuantity 
▪	TotalMarkupProfit 
▪	ExpectedRevenuePerProductQuantity 
▪	TotalExpectedRevenue 
▪	Revenue Contribution by Category 
Part 2: Product Metrics: Calculate for the following:  
•	TotalInitialQuantityOfItems 
•	TotalCurrentQuantityOfItems 
•	Num_of_ItemsSoldPerProduct 
•	Total Units Sold: Sum of InitialQuantity minus CurrentQuantity for all items or per item category. 
•	ObtainedRevenuePerProduct 
•	Total ObtainedRevenuePerProduct 
•	Which item fall under the following categories: Highest Selling and Most Profitable? 
NB: You can use your discretion to name the columns as you see fit but it must capture the metrics and KPIs given above. 
 
 
 
Part 3: Temporal Calculations 
o	PurchaseYear = YEAR (UMFSData [PurchaseDate]) 
o	PurchaseMonth = FORMAT (UMFSData [PurchaseDate], "MMMM") 
 
Part 4: Inventory Management 
UrbanMart must consider the temporal aspect of its operations. The perishable nature of many of its products necessitates precise inventory management to minimize losses from expired items and to ensure the availability of fresh products for its customers. The timing of procurement and sales also impacts costs and revenues, adding another dimension to the pricing optimization problem. 
1.	Evaluate the information available in the DaystoExpiry and ItemStatus Columns. 
▪ Product Lifecycle Metrics 
❖	Number of Fresh Products: Count of items where ItemStatus is 'Fresh'. 
❖	Number of Near Expiry Products: Count of items where ItemStatus is 'Near Expiry'. 
❖	Total Expired Products 
2.	What is the distribution of 'Days to Expiry' across different item categories? Are there categories with higher risk of product expiry? 
3.	How does the 'Days to Expiry' affect the selling price and profitability of items?  
4.	Stock Levels: How does UrbanMart's current stock level for each item compare to the initial stock? Are there items that are overstocked or understocked? 
5.	What do you think about the financial position of the company? Refer to Q.3 
All the best.  
 

