# Car Sales Analysis - Power BI Project

## Dataset Overview
**Dataset Name:** Car Sales  
This dataset contains key information related to car sales, including details about the car, customer, dealer, and sales transactions. Below are the columns used in the dataset:
- **Car_id:** Unique identifier for each car sold.
- **Date:** Date of the transaction.
- **Customer Name:** Name of the customer.
- **Annual Income:** Annual income of the customer.
- **Dealer_name:** Name of the dealer responsible for the sale.
- **Company:** The company or brand of the car.
- **Model:** The specific model of the car.
- **Engine:** Engine specifications of the car.
- **Transmission:** Type of transmission (e.g., manual, automatic).
- **Colour:** Color of the car sold.
- **Price:** Price at which the car was sold.
- **Dealer_No:** Identification number for the dealer.
- **Body Style:** Style of the car body (e.g., sedan, SUV).
- **Phone:** Contact number of the dealer.
- **Dealer_region:** The region where the dealer operates.

![image](https://github.com/user-attachments/assets/0e14da9a-4f1a-4c2f-b6a3-c9046e011ccd)

---

## Project Workflow

### Step 1: Data Cleaning & Manipulation
In the initial step, I performed **data cleaning and transformation** using **Power BI Power Query**. This involved tasks like:
- **Removing duplicates** to maintain data uniqueness.
- **Handling missing values** for key columns to ensure accurate analysis.
- **Standardizing entries** such as dealer names and car models for consistency across the dataset.
- **Converting data types** to appropriate formats (e.g., date columns) for seamless analysis.

### Step 2: Calendar Table Creation
To ensure accurate time-based analysis, I created a **Calendar Table** using **DAX functions**. This new table contained unique date values, which served as the basis for time-related calculations such as YTD (Year to Date), MTD (Month to Date), and YoY (Year on Year) comparisons.  
The calendar table enabled the analysis to be dynamic and scalable across different time periods.

![image](https://github.com/user-attachments/assets/3c73b85a-4cc5-4eaa-93c1-e9f8406cd2d4)


### Step 3: Data Modeling
After creating the **Calendar Table**, I connected it with the **Car Sales Data** by modeling the relationship between the **Date** column in both tables. This step ensured the seamless interaction of date-based measures and visualizations.

![image](https://github.com/user-attachments/assets/93cfc5ec-4c01-4c10-aa9b-f26da3fd8431)

### Step 4: Measure Creation Using DAX
I used **DAX (Data Analysis Expressions)** to create several custom measures that provided deeper insights into sales performance. These measures include:
- **YTD Total Sales:** Year-to-date total sales.
- **YTD Cars Sold:** Year-to-date total units sold.
- **YoY Sales Growth:** Year-on-year percentage growth in sales.
- **YoY Avg Price Growth:** Year-on-year growth in the average car price.
- **Total Sales:** Total revenue generated.
- **Sales Difference:** The difference in sales between time periods.
- **PYTD Total Sales:** Prior year-to-date total sales.
- **PYTD Cars Sold:** Prior year-to-date total units sold.
- **PYTD Avg Price:** Prior year-to-date average car price.
- **MTD Total Sales:** Month-to-date total sales.
- **MTD Cars Sold:** Month-to-date total units sold.
- **MTD Avg Price:** Month-to-date average car price.
- **Max Price:** Maximum price of a car sold.
- **Cars Sold Difference:** The difference in the number of cars sold between two periods.
- **Avg Price Difference:** The difference in the average price between two periods.
- **Avg Price:** Average price of the cars sold.

### Step 5: KPI Creation
To monitor the overall sales performance, I created several **KPIs** (Key Performance Indicators), focusing on:
- **YoY (Year on Year)** sales comparison, highlighting growth or decline.
- **YTD (Year to Date)** sales, showing the cumulative sales for the year.
- **MTD (Month to Date)** sales to track performance at the monthly level.
These KPIs helped provide an at-a-glance understanding of business health across multiple timeframes.

![image](https://github.com/user-attachments/assets/cf16378a-c465-44e5-bcfc-2dbe57f3b92c)

### Step 6: Area Chart Visualization
To analyze sales trends over time, I built an **Area Chart** that displayed the weekly trend of **YTD Sales**. This visualization helped in tracking sales fluctuations and seasonal trends on a week-by-week basis.

![image](https://github.com/user-attachments/assets/1eea35f7-c512-478d-bba5-178c0bbff668)

### Step 7: Donut Charts for Sales Analysis
I created two **Donut Charts** to provide detailed insights into the distribution of sales:
1. **YTD Sales by Body Style:** Visualizing the contribution of different car body styles (sedan, SUV, etc.) to overall sales.
2. **YTD Total Sales by Colour:** Showing the distribution of sales based on car colors, helping to identify customer preferences.

![image](https://github.com/user-attachments/assets/325457a8-afd3-4ae3-8150-7e517338d214)

### Step 8: Map Visualization by Region
To visualize the geographical distribution of sales, I created a **Map** that displayed the **YTD Cars Sold by Dealer_region**. This map highlighted which regions had the highest sales, providing insights into regional performance and dealer success.

![image](https://github.com/user-attachments/assets/fa319f5c-c717-4bb9-802a-39f91d1c7a12)

### Step 9: Company-wise Sales Trend Table
I developed a **Sales Trend Table** for company-wise analysis. The table compared multiple metrics such as:
- **YTD Avg Price**
- **YTD Cars Sold**
- **YTD Total Sales**
- **% Growth Target YTD Total Sales**
This comparison allowed a comprehensive understanding of how different companies performed in terms of sales, pricing, and growth targets.

![image](https://github.com/user-attachments/assets/b4064762-ef9b-4366-9587-43c964326f8f)

### Step 10: Filters and Slicers
To make the dashboard more interactive and user-friendly, I added several **Slicers** for easy filtering of the data. Users could filter the data based on:
- **Body Style**
- **Dealer Name**
- **Transmission Type**
- **Engine Specification**
This enabled more granular analysis, allowing users to explore specific aspects of the sales data.

![image](https://github.com/user-attachments/assets/5ba2cb17-68cd-4601-93be-e841b9b6216e)

### Step 11: Detailed Sales Page
I created a **Detailed Sales Page** that showcased individual car sales for each **Car ID**. This allowed a more focused view on specific sales transactions, providing deeper insights into each car's sale details.

![image](https://github.com/user-attachments/assets/7a64c675-8142-4c99-ad3b-6b93138f76d1)


### Step 12: Interactive Dashboards with Buttons
I connected both dashboards using **interactive buttons** to enhance the user experience. These buttons allowed seamless navigation between the main dashboard and the detailed sales page, making it easier for users to explore the data in depth.

![image](https://github.com/user-attachments/assets/6e802bc3-ed91-4530-8e52-a43dd12c5830)

---

## Overall Summary
In this project, I applied **more than 25 DAX functions** to generate insights and create dynamic visualizations. The project focuses on analyzing car sales performance across multiple dimensions—time, geography, company, body style, and more. Through the use of **Power BI** and **DAX**, this dashboard provides a comprehensive view of the business's sales performance and helps identify key trends and opportunities for growth.

![image](https://github.com/user-attachments/assets/7b7a2f01-7113-465d-8657-b6a8274a9f9f)

--- 

## Key Skills Utilized
- **Data Cleaning & Transformation (Power Query)**
- **DAX Calculations & Measures**
- **Data Modeling**
- **Interactive Visualizations**
- **KPI & Performance Tracking**
- **Power BI Dashboard Development**

---

