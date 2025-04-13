# 📊 ROS Analytics Project

## 🧩 Overview

This project provides comprehensive analytics for the **Restaurant Order System (ROS)** using a **KNIME workflow** (`Project_ROS1.knwf`). It processes and visualizes **Key Performance Indicators (KPIs)** to help stakeholders monitor, evaluate, and improve restaurant operations across multiple dimensions such as:

- Revenue
- Customer behavior
- Delivery performance
- Payment success

The dataset used in this project has been **collected and generated for restaurants operating in the United Kingdom (UK)**, reflecting regional dining patterns, customer behavior, and operational performance relevant to the UK market.


---

## 🧰 Workflow Platform

- **Tool**: [KNIME Analytics Platform](https://www.knime.com/)
- **File**: `Project_ROS1.knwf`
- **Format**: Visual data workflow (drag-and-drop based)

---

## 📈 Key Performance Indicators (KPIs)

### 1. 🏪 Restaurant Performance Metrics
- **Total Revenue by Restaurant**: Sum of `OrderTotal` grouped by `RestaurantID`
- **Average Order Value (AOV)**:  
  `AOV = Total Order Amount / Number of Orders`
- **Order Type Distribution**: Proportions of Dine-In, Takeaway, Home Delivery

### 2. 👥 Order & Customer Insights
- **Peak Order Hours**: Analyze `OrderDateTime` to find high-traffic hours
- **Customer Retention**: Count of customers placing multiple orders
- **Order Cancellation Rate**:  
  `Cancelled Orders / Total Orders * 100`

### 3. 💰 Tax & Revenue Insights
- **Revenue by Tax Type**: Grouped by `TaxApplicable`
- **Convenience Fee Contribution**:  
  `(ConvenienceFee / Total Revenue) * 100`

### 4. 🚚 Delivery Partner Metrics
- **Delivery Timeliness**:
  - On-Time (< 30 min)
  - Slightly Late (< 45 min)
  - Delayed (< 60 min)
  - Very Late (> 60 min)

### 5. 💳 Payment Metrics
- **Payment Success Rate**:  
  `Successful Payments / Total Payments * 100`
- **Payment Mode Distribution**: Card, Cash, UPI percentages
- **Failed Payment Analysis**: Failures by `PaymentMode` or `OrderID`

### 6. 📊 General Insights
- **Active vs Inactive Restaurants**: Count based on `Status`
- **Revenue by Cuisine**: Most profitable cuisines
- **Restaurant Performance Score**:
  - **Performance Ratio** = `Actual Revenue / Expected Revenue`
  - **Ratings**:
    - Excellent (≥ 1.0)
    - Good (0.8 – 0.99)
    - Needs Improvement (0.6 – 0.79)
    - Poor (< 0.6)

---

## 🚀 How to Use

1. Open **KNIME Analytics Platform**
2. Import the workflow: `File → Import KNIME Workflow`
3. Configure data sources (CSV, database, etc.)
4. Execute the workflow nodes
5. View tables and dashboards
6. Export results (CSV, Excel, HTML)

---

## 📂 File Structure

```bash
📁 ROS_Analytics_Project/
├── datasets           # datasets used
└── Project_ROS1.knwf                   #  KNIME workflow
