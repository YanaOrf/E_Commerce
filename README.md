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





### States 
[Dash_1](https://public.tableau.com/views/E-CommerceDashboard1/Overview?:language=en-GB&:display_count=n&:origin=viz_share_link)

### Time
[Dash_2](https://public.tableau.com/views/E-CommerceDashboard2/Customers?:language=en-GB&:display_count=n&:origin=viz_share_link)


### Clusters overview 


![clusters](https://github.com/YanaOrf/E_commerce/blob/main/scatter_hue.png)


[Dash_3](https://public.tableau.com/views/Overviewoftheclusters/Overviewoftheclusters?:language=en-GB&:display_count=n&:origin=viz_share_link)

### Overview of a typical order

[dash_4](https://public.tableau.com/views/Overviewofatypicalorder/Typicalorderoverview?:language=en-GB&:display_count=n&:origin=viz_share_link)

### Top profitable sub_categories by sales

Profitable articles are sold in small volumes.Low-margin items are sold in large quantities 

Hypothesis:

Increase the discount on marginal products to increase their sales volume

[plot](https://public.tableau.com/views/Topprofitablesub_categoriesbysales/Topprofitablesub_categoriesbysales?:language=en-GB&publish=yes&:display_count=n&:origin=viz_share_link)

Hypothesis:

* Increase the discount on marginal products to increase their sales volume

* Exclude unprofitable items from the range to increase profit margin

### Product groups according to avg. profit margin and avg. discount 

[plot](https://public.tableau.com/views/E-Commerce_16711952726490/MarginDicscount_3?:language=en-GB&:display_count=n&:origin=viz_share_link)

### Correlation between discount and sales
[dash_5](https://public.tableau.com/views/Correlationbetweendiscountsales/discountandsales?:language=en-GB&:display_count=n&:origin=viz_share_link)

## Conclusion  

According to analysis, it is posibble to increase profit margin n 35% by excluding unprofitable items () from the range


