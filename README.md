# <ins>Project Background</ins>
**Olist**, a major Brazilian e-commerce platform founded in 2015, operates as a department store marketplace, enabling thousands of merchants to sell their products on its platform and ship them nationwide. The company's business model relies on logistical efficiency and high customer satisfaction to maintain its competitive edge.

This project analyzes a real-world dataset of over 100,000 orders, between 2016 and 2018, to provide insights and recommendations on the following key business areas:

*   **Sales Performance:** Identifying the core product categories driving revenue.
*   **Logistics Benchmarking:** Analyzing delivery performance by region to pinpoint critical bottlenecks.
*   **Strategic Prioritization:** Synthesizing sales and logistics data to create a strategic framework for operational improvements.

  
# <ins>Data Structure</ins>
The project's relational database structure consists of several interconnected tables, containing over 100,000 order records. The tables directly utilized are represented through the following Entity-Relationship Diagram:
<img width="1100" height="592" alt="Blank diagram (1)" src="https://github.com/user-attachments/assets/c5225338-31b7-4190-bfe5-465ee89ee3e0" />

# <ins>Executive Summary</ins>
### **Overview of Findings**
Olist experienced explosive year-over-year (YOY) growth, with sales increasing by 140% to $13.6M. However, this rapid scaling is visibly straining our logistics network, resulting in a 2.1% increase in average delivery times.

The dashboard below summarizes this core challenge. The central 'State Performance Quadrant Analysis' segments each state into one of four strategic quadrants to identify where to focus our efforts:
*   **Quadrant 1: Critical Risk** - High-value markets where slow delivery speeds are jeopardizing major revenue streams.
*   **Quadrant 2: Best in Class** - Our top-performing markets with both high sales and fast delivery, representing the model for success.
*   **Quadrant 3: Efficient but Small** - Smaller markets with good operational performance but lower strategic priority for growth.
*   **Quadrant 4: Untapped Potential** - Underserved markets where poor logistics are suppressing a massive growth opportunity.
<img width="994" height="559" alt="Quadrant Analysis" src="https://github.com/user-attachments/assets/4e325a20-b618-4ae2-978d-32824a14a734" />

#### **Quadrant Analysis**
*   Quadrant 2 makes up for **80.83%** of total volume (indicated by bubble size). This is heavily impacted by the state of São Paulo with a delivery time of 8.7 days and a order volume of **41,746**.

# <ins>Insights Deep Dive</ins>

#### **Category 1: Sales & Revenue Performance**

*   **Main insight 1.** The business saw exceptional YOY growth across key metrics. Total Sales grew by **140.4%** to **$13.6M**, driven by a **141.3%** increase in Sales Volume (seen in graph 1).
*   **Main insight 2.** Revenue is highly concentrated in a few key product categories. "Bed, Bath & Table", "Watches" (gifts), and "Health & Beauty" are the top performers, making their operational stability critical to the company's bottom line.

      <img width="860" height="540" alt="Product Category Chart" src="https://github.com/user-attachments/assets/3f8140ac-6d91-45cc-b3d0-d2871456a462" />

#### **Category 2: Logistics & Delivery Benchmarking**

*   **Main insight 1.** The explosive growth in sales has led to a degradation in delivery performance. The overall average delivery time increased by **2.12%** YOY, indicating that our current logistics infrastructure is struggling to keep pace with demand.
*   **Main insight 2.** A severe North-South divide in logistical performance exists. The map below shows that deliveries to the South are fast and efficient with delivery times averaging around **12.01 days**. The North and Northeast regions suffer from signfiicant delays, seeing an average delivery time of **22.39 days (86% more than South region)**.

<p align="center">
<img width="468" height="452" alt="Brazil" centered="true" src="https://github.com/user-attachments/assets/2a5e2ed4-ea50-420b-b81b-9472f698b987" />
</p>


---

### **Recommendations**

1.  **Specific observation:** No states currently fall into Quadrant 1. This indicates that Olist’s highest-value markets are being supported by logistics that, while strained, are not yet undermining core revenue. This is a **good thing**, it shows the company is protecting its most important revenue streams in the midst of YoY revenue growth. 
    *   **Recommendation:** To avoid future risks of states moving beyond defined threshold (most likely Q2 moving to Q1 due to increasing delivery times), establish a logisitcs risk dashboard that flags states with increasing delivery times beyond a moderate threshold. In the same manner, introduce several "what-if" stress models (e.g., 30% increase in orders in Rio Grande Do Sul) to identify possible bottlenecks **before** they occur. **Though there is not a current risk of states entering the critical risk quadrant, proactive monitoring is essential to sustainably avoid risks while continuing to scale**.

2.  **Specific observation:** States in the Northeast consistently fall into **Quadrant 4 (Untapped Potential)**, with the worst delivery performance and correspondingly low sales.
    *   **Recommendation:** Improve delivery times in the NW by partnering with local carriers or adding a small regional hub. Start with a pilot group in one major city (ex. Amazonas) to measure the impact on delivery time and sales volume before expanding further.

3.  **Specific observation:** São Paulo ('SP') is the clear leader in **Quadrant 2 (Best in Class)**, handling our highest volume with exceptional speed.
    *   **Recommendation:** Standardize excellence by documenting the processes from this region to create a company-wide "Logistics Playbook."

---
