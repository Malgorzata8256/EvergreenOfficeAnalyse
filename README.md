# Online Shopping Behavior Analysis - Evergreen Office

---

## **Table of Contents**

1. [Project Background](#project-background)
2. [Data Structure](#data-structure)
3. [Executive Summary](#executive-summary)
4. [Insights Deep Dive](#insights-deep-dive)
5. [Recommendations](#recommendations)
6. [Assumptions and Caveats](#assumptions-and-caveats)

---

## **Project Background**

### **Company Context**
Evergreen, established in 2009, is a global company specializing in office equipment sales in Canada via its website and mobile app.

Despite its strong foothold in technology products and corporate clients, the company has experienced a **decline in sales** over the past years. This downturn, starting in 2010, continued through 2011, with a brief recovery in 2012. This has raised critical questions about the effectiveness of current strategies, prompting discussions on whether to focus marketing efforts on specific customer groups or regions, or to discontinue certain product categories.

Evergreen holds extensive data on sales, operational efficiency, product offerings, and customer distribution. However, this data has not been fully utilized to inform strategic decision-making. This project thoroughly analyzes and synthesizes these data points to uncover actionable insights aimed at improving Evergreen's commercial success.

### **Key Focus Areas**

This analysis provides insights and recommendations in the following domains:
- **Sales Trends:** Evaluating historical sales patterns with a focus on revenue, order volume, and average order value.
- **Product Performance:** Conducting a detailed analysis of product categories and individual product success, assessing contributions to revenue and order volume over time.
- **Regional Comparisons:** Examining how different regions contribute to overall performance, including sales, product preferences, and growth trends.
- **Customer Distribution:** Analyzing customer segmentation by type and geography, focusing on shifts in customer behavior and purchasing trends.

An interactive Power BI dashboard showcasing these insights is available here.

!!!!! Technical stuff!!!!

---

## **Data Structure**

The database structure, shown below, is based on a star schema and consists of four **dimensional tables**: Calendar, OrderDates, Products, Customers, as well as one **fact table** (FactOrders), containing a total of 8,399 records. The analysis spans shipped orders between **January 2009 and December 2012**.

  ![Database structure schema](Visuals/Evergreen_schema.png)

Before starting the analysis, several quality control and data exploration steps were performed using Power Query and Excel. These checks ensured data accuracy and consistency while providing familiarity with the dataset. Details of the quality checks and data validation processes can be found here.

---

## **Executive Summary**

### **Overview of Findings**

In its first year of operations, Evergreen achieved a revenue of 4.18 million USD, but subsequently experienced a notable decline in sales during the following two years—down by 15.43% in 2010 and 2.72% in 2011. While 2012 saw a sales growth of 7.73%, it is concerning that the average order value (AOV) in two key product segments—technology (-2%) and furniture (-11%)—continued to decrease. This decline, despite some recovery in 2012, can largely be attributed to a return to pre-crisis conditions.

The impact of the 2008 financial crisis, while significant in the earlier years, might have had lingering effects on market dynamics. However, the fact that Canadian financial institutions operate under stricter regulations, suggests that the direct impact of the U.S. financial crisis on Canadian businesses like Evergreen should have been somewhat mitigated by these regulatory safeguards. The following sections will further investigate additional contributing factors and identify key opportunities for improvement.

Below is the overview page from PowerBI dashboard and more examples are included throught the report. The entire interactive dashboard can be downloaded here. 

![Overview Sales](Visuals/SalesOverviewPage.png)

---

## **Insights Deep Dive**

### **Sales Trends**

- Evergreen's sales trends demonstrate significant variability since the company’s launch in 2009. **The inaugural year began strong, with the highest revenue recorded in January at $506,597 from 144 orders.** However, sales quickly fluctuated, **dropping to $230,767 in May** and recovering to $409,164 in December.

- **2010 saw a general decline in sales, finishing 15.43% lower than 2009**. The year started with weak performance and experienced sharp drops in July and August. Despite this, **the final quarter of 2010 achieved the best results of the year, generating $1,022,036 in revenue**.

- **In 2011, sales hit their lowest point in June, with revenue of $197,941.** Although the last quarter was again the strongest, overall annual performance remained weaker compared to prior years. A notable finding is that **consumer orders increased slightly (+5.82%), but revenue from these orders dropped significantly (-27.92%)**. Small business clients showed a similar pattern, with a small rise in order volume but a decrease in revenue.

- **2012 marked some recovery, with an overall sales increase of 7.73% compared to 2011.** Improvements were particularly notable in the consumer and small business segments, driven by strategic changes in free delivery policies. For instance, consumer orders rose by +33.33%, while revenue from these orders increased by +127.8%, likely reflecting the impact of the higher free delivery threshold introduced in 2012. In the small business segment, the earlier introduction of this policy in 2011 resulted in sustained growth, with a +9.93% increase in revenue and a +6.88% rise in orders in 2012. Despite these gains, several months in 2012 still underperformed compared to earlier benchmarks from 2009.

- Recurring sales patterns in Evergreen demonstrate significant variability, with peak performance often occurring either in the final quarter or the first quarter of the year. While end-of-year peaks are typically followed by weaker first quarters, there are also instances where strong first-quarter performance corresponds with a softer preceding fourth quarter. These fluctuations are likely driven by client behaviors such as tax planning and budget adjustments, particularly among corporate and small business clients, who may adjust their purchasing strategies based on annual financial results.

### **Product Performance**

### **Regional Comparisons**

### **Customer Distribution**


- 
- The **West Region** leads in sales across all categories but has the largest share of **technology products**.
- **Office Supplies** have a disproportionate share of orders in all regions but do not translate to equivalent revenue. This raises questions about **profitability and operational costs** for this category.

| Region   | Total Sales (2009-2012) | Dominant Category | Avg. Order Value |
| -------- | ----------------------- | ----------------- | ---------------- |
| West     | $6.4M                  | Technology        | $2,850          |
| Central  | $4.5M                  | Technology        | $2,750          |
| Atlantic | $2.0M                  | Office Supplies   | $870            |
| North    | $1.9M                  | Office Supplies   | $840            |

### **2. Product Performance**

- Top-performing product (by value): **Polycom ViewStation ISDN Videoconferencing Unit** ($265,794 in sales).
- Top-performing product (by volume): **Global High-Back Leather Tilter Chair** (666 units sold).
- **Office Supplies** products have the highest order count but generate the lowest revenue. Costs associated with fulfillment should be reviewed.

### **3. Customer Behavior**

- Corporate customers placed 2,100 orders (50% higher than other segments).
- **Small Businesses** and **Home Office** customers show potential for growth with targeted marketing strategies.

---

## **Recommendations**

1. **Product Portfolio Optimization:**

   - Evaluate **Office Supplies** profitability. High order volumes and low average order values indicate a potential strain on operational efficiency.
   - Focus on promoting high-margin products in **Technology** and **Furniture**.

2. **Regional Marketing Strategies:**

   - Target the **West Region** with technology-based promotions to leverage existing trends.
   - Develop specific campaigns for **North and Atlantic Regions** to improve sales and customer engagement.

3. **Customer Segmentation:**

   - Strengthen marketing for **Corporate Clients**, who drive the majority of sales.
   - Provide personalized offers to **Small Businesses** to increase their share of revenue.

4. **Operational Efficiency:**

   - Assess the cost structure of **Office Supplies** orders. Consider consolidation or minimum order requirements to reduce costs.

5. **Sales Recovery Plan:**

   - Capitalize on the 2012 recovery trend with seasonal promotions and loyalty programs.
   - Investigate the impact of shipping speed and explore expedited delivery options to enhance customer satisfaction.

## **Assumptions and Caveats**
