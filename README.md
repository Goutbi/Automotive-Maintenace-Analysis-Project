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
![Screenshot 2024-10-13 202818](https://github.com/user-attachments/assets/db928339-8f9e-4ae0-b345-25a2a35d229f)

<div class='tableauPlaceholder' id='viz1728881797305' style='position: relative'><noscript><a href='#'><img alt='Dashboard 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;ca&#47;carmaintenance&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='carmaintenance&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;ca&#47;carmaintenance&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1728881797305');                    var vizElement = divElement.getElementsByTagName('object')[0];                    if ( divElement.offsetWidth > 800 ) { vizElement.style.minWidth='420px';vizElement.style.maxWidth='650px';vizElement.style.width='100%';vizElement.style.minHeight='587px';vizElement.style.maxHeight='887px';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.minWidth='420px';vizElement.style.maxWidth='650px';vizElement.style.width='100%';vizElement.style.minHeight='587px';vizElement.style.maxHeight='887px';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';} else { vizElement.style.width='100%';vizElement.style.height='977px';}                     var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

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
