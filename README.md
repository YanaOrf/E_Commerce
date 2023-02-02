# E_commerce
![logo](https://melchers-china.com/wp-content/uploads/2020/07/1-1.jpg)

## Data source

the [file](https://drive.google.com/file/d/1j3BVqD5_KDfvXdljnZ7beV-G-FVS8df5/view) contains the dataset pertaining to 10K records of information about:
* Date of the order and the shipment 
* Shipment Mode
* Customer Id,name,segment
* Adress of the customer (country,state,city,postel code)
* Product Id,name, category,sub-category
* Sales
* Discount
* Profit
* Quantity
  
## Project Introduction

The project focused on exploratory data analysis and database design (SQL), identification of data-driven business strategies and their presentation in an  interactive Tableau dashboard.

## Data base design 

On the firs step, I created a  [data_base](https://github.com/YanaOrf/E_commerce/blob/main/E-commerce.ipynb) using SQLite &Python and made a [ERD](https://github.com/YanaOrf/E_commerce/blob/main/ERD%20E-Commerce%20(crow's%20foot)%20-%203.png). For further analysis I performed some queries. 


## Explaroty data analysis  
In EDA I imvestigated:

* [states](https://public.tableau.com/views/E-CommerceDashboard1/Overview?:language=en-GB&:display_count=n&:origin=viz_share_link) which have made the highest number of orders and highest revenue and profit;
*  [customer buying pattern depending on the time of year](https://public.tableau.com/views/E-CommerceDashboard2/Customers?:language=en-GB&:display_count=n&:origin=viz_share_link);
*  the worst and the best sub-categories:
   *   in terms of profit margin and [sales](https://public.tableau.com/views/Topprofitablesub_categoriesbysales/Topprofitablesub_categoriesbysales?:language=en-GB&publish=yes&:display_count=n&:origin=viz_share_link);
   *   in terms of profit margin and provided [discount](https://public.tableau.com/views/E-Commerce_16711952726490/MarginDicscount_3?:language=en-GB&:display_count=n&:origin=viz_share_link)
*  [typical order overview](https://public.tableau.com/views/Overviewofatypicalorder/Typicalorderoverview?:language=en-GB&:display_count=n&:origin=viz_share_link): 
   * The most frequently purchased product sub-categories together;
   * Orders destribution according to number of categories in the order; 
   * sub-categories by delivery mode
 * [correlation](https://public.tableau.com/views/Correlationbetweendiscountsales/discountandsales?:language=en-GB&:display_count=n&:origin=viz_share_link) between  discount and sales
  
Additionaly, to understand the customers buying pattern  3 parameters were calculated : 
* Monetary
* Frequency 
* Recency (how many days has passed from the last order date in the dataset to customers last purchase)

## ML Clustering with K-means

To find meaningful structure, explanatory underlying processes, generative features, and groupings inherent in a set of examples I used unsupervised learning method - Clustering with K-means.

After removing outlires, feature scaling I used The Elbow Method and Silhouette Analysis to determine the optimal number of clusters into which the data may be clustered. 

After obtaining the optimal number of clusters (4), I used the K-means clustering algorithm to divide the clients into 4 clusters according to Monetary,Frequency,Recency. 

![clusters](https://github.com/YanaOrf/E_commerce/blob/main/scatter_hue.png)

To understand customer clusters, I researched what products customers from different [clusters](https://public.tableau.com/views/Overviewoftheclusters/Overviewoftheclusters?:language=en-GB&:display_count=n&:origin=viz_share_link) were buying.


_________



