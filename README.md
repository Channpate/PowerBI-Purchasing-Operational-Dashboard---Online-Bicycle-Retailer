# [Power BI] Purchasing Operational Dashboard - Online Bicycle Retailer

Author: Mai Ngoc Chau  
Date: 2025-04-02  
Tools Used: Power BI

---

## 📑 Table of Contents  
1. [📌 Background & Overview](#-background--overview)  
2. [📂 Dataset Description & Data Structure](#-dataset-description--data-structure)  
3. [🧠 Design Thinking Process](#-design-thinking-process)  
4. [📊 Key Insights & Visualizations](#-key-insights--visualizations)  
5. [🔎 Final Conclusion & Recommendations](#-final-conclusion--recommendations)

---

## 📌 Background & Overview  

### Objective:
### What is this project about? 

 This project analyzes purchasing scenario of a fictious bicycle manufacturer. The objective is

✔️ Provide a live picture of procurement activities to support leadership in making quick and effective decisions.

✔️ Track accurate time and quantity ordering results and evaluate supplier performance.

✔️ Analyze procurement costs to optimize and identify cost savings opportunities.

### Who is this project for?  

- Data analysts & business analysts
- Purchasing Manager  

---

## 📂 Dataset Description & Data Structure  

### Data Source  
* Source:
  * The dataset is taken from **AdventureWorks 2019 Sample Datasets**. The AdventureWorks database supports standard online transaction processing scenarios for a fictitious bicycle manufacturer (Adventure Works Cycles). Scenarios include Manufacturing, Sales, Purchasing, Product Management, Contact Management, and Human Resources.
  * This project will only query on specific tables of the database, as mentioned in the next part.
* Size: 60+ Tables
- Format: .csv

### 📊 Data Structure & Relationships  

#### 1️⃣ Tables Used:  

|Schema | Table Name | Rows | Columns |
|-------------|----------|-------------|-------------| 
| Product     | Product.Product       | 121317 | 11 |
| Product     | Product.ProductTable  | 16 | 11 |
| Purchasing  |Purchasing.ProductVendor | 460 | 11 |
| Purchasing  |Purchasing.Vendor        | 104 | 8 |
| Purchasing  |Purchasing.PurchaseOrderHeader| 4012 | 13 |
| Purchasing  |Purchasing.PurchaseOrderDetail| 8845 | 11 |

#### 2️⃣ Table Schema & Data Snapshot  

**Table 1: Orders** 


**Table 2: People** 


**Table 3: Returns**


#### 3️⃣ Data Relationships:  
👉🏻 Include a screenshot of Data Modeling to visualize relationships.  

---

## 🧠 Design Thinking Process  

Explain the step-by-step approach taken to solve the problem.  

👉🏻 Insert a screenshot of the Design Thinking steps (Screenshot your Excel design thinking tables for better presentation).  

1️⃣ Empathize  
2️⃣ Define point of view  
3️⃣ Ideate  
4️⃣ Prototype and review  

---

## ⚒️ Main Process

1️⃣ Data Cleaning & Preprocessing with Power Query
2️⃣ Data Modeling and Create measures, parameters with DAX
3️⃣ Visualize dashboard

---

## 📊 Key Insights & Visualizations  

### 🔍 Dashboard Preview  

#### 1️⃣ Dashboard 1 Preview  

![Page 1](https://github.com/Channpate/PowerBI-Purchasing-Operational-Dashboard---Online-Bicycle-Retailer/blob/af2e987ec5ad723c5ac1a37115ab16788f7775b5/Dashboard%20Capture/pj3-page1-executive-summary.png)

📌 Analysis 1:  
- **Observation:**
  - The total purchase value (Purchase Volume) reached over 70 million USD, showing a large scale of purchase, reflecting high production and sales levels.
  - The quantity of goods ordered (Demand Quantity) reached 2.3 million units, showing that production activities were very active and diversified.
  - The purchase volume was mainly distributed to categories such as Small Components, Tires, and Brakes, focusing on core components for bicycle production.

- **Recommendation:**
  - Prioritize cost control in categories with high purchase value to optimize input costs.
  - Assess seasonal demand for each category to plan orders more effectively.

#### 2️⃣ Dashboard 2 Preview  

![Page2](https://github.com/Channpate/PowerBI-Purchasing-Operational-Dashboard---Online-Bicycle-Retailer/blob/af2e987ec5ad723c5ac1a37115ab16788f7775b5/Dashboard%20Capture/pj3-page2-purchase-order-performance%20.png)

📌 Analysis 2:   
- **Observation:**
  - The on-time delivery rate is 99.95%, showing that the operation and logistics system is very efficient.
  - The return rate is 3.12%, the highest in the Components and Accessories group (over 3.3%), indicating that there is a problem with the quality of input products.
  - The average order processing time (Lead Time) is about 9 days, which is relatively reasonable, but some vendors still have higher lead times.
    
- **Recommendation:**
  - Tăng cường kiểm soát chất lượng đầu vào, đặc biệt ở danh mục linh kiện, để giảm tỷ lệ trả hàng và chi phí liên quan.
  - Làm việc với các vendor có lead time cao để cải thiện hoặc thay thế bằng nhà cung cấp nhanh hơn.

#### 3️⃣ Dashboard 3 Preview  

![Page 3](https://github.com/Channpate/PowerBI-Purchasing-Operational-Dashboard---Online-Bicycle-Retailer/blob/af2e987ec5ad723c5ac1a37115ab16788f7775b5/Dashboard%20Capture/pj3-page3-cost-performance.png)

📌 Analysis 3:  
- **Observation:**
  - Total Savings/Losses were negative $16.65K, indicating that some purchases were not at optimal prices.
  - There were some products that recorded high losses such as LL Crankarm, ML Crankarm, reflecting inefficiencies in negotiations or timing of purchases.
  - In contrast, clothing groups such as Short-Sleeve Jersey and Sports Shorts resulted in large cost savings, each up to nearly $250K.
  
- **Recommendation:**
  - Renegotiate purchase prices for loss-making components, especially crankarms and tires.
  - Increase purchasing proportion in high-savings items (such as sportswear), if market demand supports it.
  - Apply a "Buy in Bulk" strategy to products with high price volatility to ensure lowest costs.
    
#### 4️⃣ Dashboard 4 Preview  

![Page 4](https://github.com/Channpate/PowerBI-Purchasing-Operational-Dashboard---Online-Bicycle-Retailer/blob/af2e987ec5ad723c5ac1a37115ab16788f7775b5/Dashboard%20Capture/pj3-page4-vendor-performance.png)

📌 Analysis 4:  
- **Observation:**
  - There are 104 suppliers, of which 89.42% are ranked Preferred Vendor, demonstrating that the purchasing department has a stable supplier network.
  - However, the number of vendors with orders is decreasing over time, which may lead to the risk of relying on fewer suppliers.
  - Some vendors have a high return rate of over 5%, such as Signature Cycles, Crowley Sport, Mitchell Sports.
  
- **Recommendation:**
  - Diversify suppliers, especially in high-risk categories, to avoid dependence on a single source.
  - Eliminate or improve relationships with vendors with high Return Rate and low Credit Rating.
  - Set periodic KPIs for vendors such as: % On-time Delivery, Return Rate <3%, Standardized Lead Time.

#### 5️⃣ Dashboard 5 Preview  

![Page 5](https://github.com/Channpate/PowerBI-Purchasing-Operational-Dashboard---Online-Bicycle-Retailer/blob/af2e987ec5ad723c5ac1a37115ab16788f7775b5/Dashboard%20Capture/pj3-page5-product-dive-deep.png)

📌 Analysis 5:  
- **Observation:**
  - There is a positive correlation between Purchase Volume and Freight Cost: larger orders have higher shipping costs, but there is no sign of economies of scale.
  - Some shipping methods (Ship Method 2, 4) result in losses in savings, while Ship Method 1 brings significant savings.
  - Avg Freight Cost does not decrease proportionally as order value increases, indicating an opportunity to improve logistics costs.
  
- **Recommendation:**
  - Negotiate shipping terms with vendors based on larger order sizes.
  - Consider consolidating orders with more efficient shipping methods such as Ship Method 1.
  - Combine smaller orders to optimize shipping routes and avoid high marginal costs.

---

## 🔎 Final Conclusion & Recommendations  

The company's overall procurement performance shows efficient operations, with high on-time delivery rates and a stable supplier network. However, there are still many opportunities to optimize costs and improve supply chain efficiency, especially in the components and transportation categories.

✔️ To improve overall efficiency, the company should focus on:

✔️ Optimizing import prices by renegotiating with high-priced suppliers and prioritizing items that bring savings.

✔️ Controlling input quality to reduce returns and improve supplier reliability.

✔️ Diversifying suppliers, reducing dependency risks and improving logistics terms to save on transportation costs.

**📌 Key Takeaways**

💰 Large Purchase Volume (~$70M) but negative savings/losses ⇒ need to optimize purchase prices, especially in the small component group.

🚚 On-time delivery rate is very high (99.95%), but return rate >3% in some categories ⇒ need to improve quality control.

🧾 Shipping costs are not optimized for scale, opening up opportunities for negotiation and order consolidation to reduce logistics costs.

🤝 The number of vendors is decreasing, although most of them meet the standards ⇒ need to diversify supply sources, limit the risk of dependence.
