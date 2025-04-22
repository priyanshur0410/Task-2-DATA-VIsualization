# 🍕 Pizza Sales Visualization with Power BI

## 📌 Objective  
Analyze and visualize pizza sales data using Power BI to uncover daily trends, including:  
1. **Total Sales per Day** (Revenue generated daily).  
2. **Total Quantity Sold per Day** (Number of pizzas sold daily).  

---

## 🛠 Tools Used  
- **Power BI Desktop** (Free tool for data visualization).  
- **Dataset**: `pizza_sales.xlsx` or `pizza_sales.csv`.  

---

## 🚀 Quick Start Guide  

### 1. Prepare Your Dataset  
Ensure your dataset has the following columns:  
- `order_date`: Date of the order (e.g., `2023-05-01`).  
- `quantity`: Number of pizzas sold.  
- `unit_price`: Price per pizza.  

**Example Data**:  
| order_date | quantity | unit_price | pizza_type     |  
|------------|----------|------------|----------------|  
| 2023-05-01 | 2        | 12.5       | Margherita     |  
| 2023-05-01 | 1        | 15.0       | Pepperoni      |  

---

### 2. Steps to Create the Report in Power BI  

#### Step 1: Load Data into Power BI  
1. Open Power BI Desktop.  
2. Click **Home** > **Get Data** > **Excel/CSV** and select your `pizza_sales` file.  
3. Load the data into Power BI.  

#### Step 2: Data Cleaning (Optional)  
- Use **Power Query Editor** to:  
  - Ensure `order_date` is in `Date/Time` format.  
  - Remove duplicates or irrelevant columns.  

#### Step 3: Create Metrics  
1. **Total Sales**:  
   Total Sales = SUMX(pizza_sales, pizza_sales[quantity] * pizza_sales[unit_price])


Total Quantity = SUM(pizza_sales[quantity])  
Step 4: Build Visualizations
Total Sales per Day:

Drag order_date to the X-axis.

Drag Total Sales to the Y-axis.

Choose a Line Chart or Area Chart.

Total Quantity Sold per Day:

Drag order_date to the X-axis.

Drag Total Quantity to the Y-axis.

Choose a Bar Chart or Column Chart.

Step 5: Format the Report
Add titles, axis labels, and adjust colors from the Format pane.

Use Slicers (e.g., filter by pizza type).

Step 6: Save and Share
Save the report as .pbix and publish to Power BI Service (cloud) for sharing.
