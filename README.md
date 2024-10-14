# Car Maintenance Service Data Analysis

## Overview

This project analyzes data from a car maintenance service company that outsources repairs to third-party suppliers. The company collects cars from customers, manages the repair process, and delivers them back. The analysis focuses on identifying key performance indicators (KPIs) to measure growth, sales, and operational efficiency across several dimensions, including regional performance, car brand, and supplier efficiency.

Key analysis areas include:
- **Yearly Growth and Sales Analysis**
- **Regional Analysis**
- **Car Brand & Model Analysis**
- **Supplier Analysis**
- **Customer Satisfaction Analysis**

## Project Structure

The project consists of several interrelated tables representing the core business operations:

1. **Customer Data**: Information about customers (Customer ID, Name, Location, etc.).
2. **Car Data**: Details of cars associated with customers (Car ID, Brand, Model, Year).
3. **Sales Data**: Information related to sales quotations and invoices (Quotation Number, Customer ID, Invoice Amount).
4. **Service Data**: Records of services provided to cars, along with supplier involvement (Job ID, Car ID, Supplier ID, Parts & Labor Costs).
5. **Supplier Data**: Information about third-party suppliers (Supplier ID, Location, Speciality).

### Entity-Relationship Diagram (ERD)

The dataset is structured using the following relationships:
- **CustomerID** links to the customer's car data and sales data.
- **CarID** links to the service data to track repairs.
- **SupplierID** is linked to each service job to track supplier involvement and performance.

## Tableau Dashboard

You can view the full interactive Tableau dashboard directly [here](https://public.tableau.com/views/carmaintenance/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link).

(<div class='tableauPlaceholder' id='viz1728886018570' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;ca&#47;carmaintenance&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='path' value='views&#47;carmaintenance&#47;Dashboard1?:language=en-US&amp;:embed=true&amp;:sid=&amp;:redirect=auth' /> <param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;ca&#47;carmaintenance&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div><script type='text/javascript'>                    var divElement = 

## Key Insights

### 1. Sales Trends
- **Observation**: Sales have shown consistent growth over time, with noticeable peaks during certain months.
- **Recommendation**: Capitalize on these trends by offering seasonal promotions.
- **Suggested Visualization**: A line graph showing monthly or yearly sales growth (Invoice Amount).

### 2. Regional Analysis
- **Observation**: Most sales occur in Khartoum, while regions like Bahri and Omderman are underrepresented but growing.
- **Recommendation**: Focus marketing efforts on regions with potential for growth, such as Bahri and Omderman.
- **Suggested Visualization**: A bar chart showing total sales by region.

### 3. Product (Car Brand & Model) Analysis
- **Observation**: Brands like Toyota and Kia are the most frequently serviced, with models like the Camry and Optima leading the list.
- **Recommendation**: Offer targeted service packages for popular car brands.
- **Suggested Visualization**: A stacked bar chart showing the frequency of services by car brand and model.

### 4. Supplier KPI Metrics
- **Observation**: Suppliers specializing in engine repairs show higher customer satisfaction.
- **Recommendation**: Track supplier performance using KPIs such as average service completion time, cost per job, and customer ratings. Use this to negotiate better rates or replace underperforming suppliers.
- **Suggested Visualization**: A bar chart showing supplier efficiency by average customer ratings and total repair costs.

## Installation and Usage

### Prerequisites
- Python 3.x
- Pandas
- Matplotlib
- Seaborn
- SQLAlchemy (or any database connection tool)
- Jupyter Notebook (optional for analysis)

### Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/car-maintenance-analysis.git
   cd car-maintenance-analysis
