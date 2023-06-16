#  Exploratory Data Analysis - Super Store Retail
As a business manager, we will try to find out the weak areas where we can work to make more profit.
what all business problems we can derive by exploring the data?

We will create a Power BI Dashboard using the dataset [Superstore](https://drive.google.com/file/d/1lV7is1B566UQPYzzY8R2ZmOritTW299S/view).

![Overview Page of Dashboard](screenshots/1.png)
___
## This project will be split into 2 parts:
- data preprocessing: Using Power Query and M-language where we will split our one large 10000 records and 13 wide columns into star schema for better analysis and performance.
  
- [Power BI Dashboard](./SuperStore.pbix): showing the analysis of the data and the insights we can derive from it.
  ___

## Part 1:  Data Preprocessing: 
After Exploring the data and modeling the Data here is the star schema used for developing the dataset

![Schema](screenshots/Schema.png)

- There were no Date/Time Data, so we would be limited to analyzing 3 facts [Sales, Profit, Quantity].
  - based on different dimensions [Shipment Mode, Customer Segment, Geo-location, Product Category]
  - Analyze the effect of Discount on Sales and profit
___
## Part 2: Data Exploration and Analysis Dashboard
  - firstly we provided **General insights**:
  - The Store has delivered \$38K product across 9994 orders with an average 3.79 Product per order.
  - Accomplished total Profit of 288K from Sales of \$2.3M, with an average  \$230 per order and $29 per product Price.
  ![Sales Report](screenshots/1.png  "2015 was the most active year across all Time Period") ![avg analysis](screenshots/21.png  "2015 was the most active year across all Time Period")


- **secondly we presented Category Insights**:
     - With products span across 3 categories, the Office Supplies is most sold products with 22,981 sold products which represent 60.5% of total sales, followed by Technology and Furniture with ~8,000 sales each.
     -  The most sold products are the Binders with 6,010 sold products, followed by Paper with 5,192 sold products, both belongs to office supplies.
     - While the Office Supplies is the most sold category in quantity, it is not the most profitable, this place is occupied with Technology with the highest sales around \$839k and highest profit with \$146K.
     - Another interesting fact is that the Furniture category is the least profitable category with only \$19k profit from 720k sales, in fact we can see that both Tables (\$207k sales and \$17 loss in profit) and Bookcases (\$115k sales and $4k loss in profit) are the most losing products.
     - On the other hand we can see that the most profitable products belongs to technology category, with the Copiers as the most profitable product with \$150k sales and \$56k profit, followed by Phones with \$331k sales and \$45k profit, and Accessories with \$167k sales and \$42k profit.
      ![Category Analysis](screenshots/21.png)

- **also we  produced Products and Geo-graphical insights**:
    - The most profitable products is Copiers and Phones with \$56k and \$45k profit respectively and the most losing products are Tables and Bookcases with \$18k and \$4k loss respectively.
    - The most profitable state is California with \$76k profit, followed by New York with \$71k profit, and the most losing state is Texas with \$25k loss, followed by Ohio with \$18k loss.
    -  The most profitable city is New York City with \$65k profit, followed by Los Angeles with \$34k profit, and the most losing city is Philadelphia with \$15k loss, followed by Houston with \$14k loss.
  ![Group Insight Page 2](screenshots/37.png)
  ![Group Insight Page](screenshots/31.png)
  ![Group Insight Page 2](screenshots/34.png)

- **Finally we examined the effect of remaining dimensions on the sales facts**:

  - **Shipment Mode**:
    - The most used shipment mode is Standard Class with 59% of total orders, followed by Second Class with 19% of total orders, and the most profitable shipment mode is First Class with \$31k profit, followed by Second Class with \$29k profit.
    - shipping mode has no effect on the sales and profit.
  ![Group Insight Page 2](screenshots/102-1.png)
  
  - **Customer Segment**:
    - The most profitable customer segment is Home Office with \$60k profit, followed by Corporate with \$60k profit, and the most losing customer segment is Consumer with \$11k loss.
    - the customer segment has no effect on the sales and profit.
  ![Group Insight Page 2](screenshots/102-2.png)
    
  - **Discounts**:
    - As we can see that all of discounts above 30% are losing money, and the most losing discount is 80% with \$2k loss, followed by 70% with \$1.5k loss, and the most profitable discount is 10% with \$7k profit, followed by 20% with \$6k profit.
     - We can suggest limiting the discount to 20% to maximize the profit, avoid discount above 30% to avoid losing money.
     - We can also suggest following another marketing strategies instead of  discounting, such as offering free shipping, or offering free gift with the order.
     - Higher discounts have no effect on the sales or quantity while effecting the branding image, showing the product as low quality.
  ![Group Insight Page 2](screenshots/101-1.png)
  ![Group Insight Page 2](screenshots/101-2.png)
  ![Group Insight Page 2](screenshots/101-3.png)
  ![Group Insight Page 2](screenshots/101-4.png)
___
## Dashboard
Due to limitation of sharing Power BI dashboard, I will share the screenshots of the dashboard and the link to the dashboard.
[SuperStore.pbix](./SuperStore.pbix)

### Dashboard Screenshots
#### 0-Home Page:
![Dashboard Overview](screenshots/0.png)

___

#### 1- Sales Report:
![Dashboard Overview](screenshots/1.png)
![Dashboard Country](screenshots/2.png)
![Dashboard Country](screenshots/3.png)
![Dashboard Country](screenshots/4.png)
![Dashboard Country](screenshots/6.png)
![Dashboard Country](screenshots/5.png)

___
#### 2- Category Analysis:
![Dashboard Group](screenshots/21.png)
![Dashboard Group](screenshots/22.png)
![Dashboard Group](screenshots/23.png)

##### 3- Product Analysis:
![Dashboard Group](screenshots/31.png)
![Dashboard Group](screenshots/32.png)
![Dashboard Group](screenshots/33.png)
![Dashboard Group](screenshots/34.png)

##### Insights 1 - Sales and Profit by Category:
![Dashboard Group](screenshots/41.png) 
![Dashboard Group](screenshots/42.png) 

##### Insights 2 - Sales and Profit by Products:
![Dashboard Group](screenshots/51.png)
![Dashboard Group](screenshots/52.png)
![Dashboard Group](screenshots/53.png)
![Dashboard Group](screenshots/54.png)
![Dashboard Group](screenshots/55.png)

##### Insights 3 - Sales and Profit by State:
![Dashboard Group](screenshots/61.png)
![Dashboard Group](screenshots/62.png)
![Dashboard Group](screenshots/63.png)
![Dashboard Group](screenshots/64.png)
![Dashboard Group](screenshots/65.png)

##### Findings:
![findings](./screenshots/findings.png)


Please refer to the 
- [Superstore.pbix](./SuperStore.pbix) for more details.
  - The dashboard is interactive, you can click on any of the charts to filter the data.

P.S: This Dashboard was developed as part of the Spark Foundation Internship Program, and it is intended to be used as a show case study.
