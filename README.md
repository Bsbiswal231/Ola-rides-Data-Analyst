# Ola Rides Analysis Dashboard:(Excel, SQL & Power BI Project).

### Project Overview:

- This project provides a comprehensive data analysis solution for a ride-sharing service (Ola Rides), focusing on Operational Efficiency, Revenue Generation, and Service Quality. The solution uses a Data Preparation Pipeline that involves SQL for robust data cleaning and calculation, and Power BI for dynamic visualization and dashboard development.
- Tools Used: Excel, SQL (for querying), Power BI (for visualization).
- Goal: To transform raw ride-sharing transaction data into five distinct, actionable dashboards that provide data-driven insights for management and operations teams.

### Dataset Used:
<a href="https://github.com/Bsbiswal231/Ola-rides-Data-Analyst/blob/main/Ola%20rides.csv"> Ola Rides Data </a>

### Key Analytical Focus Areas & KPIs:
#### The project is structured around five critical areas of business performance, driving the dashboard design:
##### 1. Overall:
- Ride Volume Over Time, Booking Status Breakdown.
##### 2. Vehicle Type:
- Avg. Ride Distance, Avg. Customer Ratings by Vehicle Type.
##### 3. Revenue:
- Total Booking Value, Revenue by Payment Method, Top 5 Customers.
##### 4. Cancellation:
- Cancelled Rides Reasons (Customer & Driver).
##### 5. Ratings:
- Driver Ratings Distribution, Customer vs. Driver Ratings.
  
### Data Preparation and Transformation (SQL):
- A crucial step in this project was using SQL to clean, aggregate, and calculate key business metrics before loading the data into Power BI.
  
### Key SQL Operations Performed:
- 1. Successful Bookings: Retrieve all records where booking_status='Success'.
- 2. Vehicle Performance: SELECT vehicle_type, AVG(ride_distance_km) AS avg_ride_distance (to find average distance per vehicle type).
- 3. Cancellation Analysis (Customer): SELECT SUM(cancelled_rides_by_customer) AS Total_rides_cancelled_by_customer.
- 4. Top Customers: SELECT customer_id, COUNT(booking_id) AS Total_rides (Grouped and ordered to find Top 5).
- 5. Cancellation Analysis (Driver): Calculated cancellations due to specific reasons (e.g., 'Personal & Car related issues').
- 6. Ratings: SELECT MAX(driver_ratings), MIN(driver_ratings) for specific vehicle types (e.g., 'Prime Sedan').
- 7. Revenue: SELECT SUM(booking_value) AS Total_booking_values for successfully completed rides.
- 8. Incomplete Rides: Listed incomplete rides and their associated reasons.
##### SQL QUERIES: 
<a href="https://github.com/Bsbiswal231/Ola-rides-Data-Analyst/blob/main/Sql-Queries.pdf"> Sql Queries </a>

### Dashboard Design and Insights (Power BI):
- The project features five dedicated, interactive dashboards, providing a granular view of every operational aspect.
  
#### 1. Dashboard-1: Overall Performance:
- Focus: A high-level operational overview and health check.
- Key Visuals: Ride Volume Over Time (Line Chart), Booking Status Breakdown (Donut Chart).
- Insight: Clearly tracks demand trends and quantifies the operational success rate of bookings versus cancelled/incomplete rides.
<img width="1131" height="648" alt="Dashboard - 1" src="https://github.com/user-attachments/assets/680bfbcf-9346-4fb9-81a3-5c8b0c7de704" />

#### 2. Dashboard-2: Vehicle Type Analysis:
- Focus: Evaluating the performance and quality specific to vehicle segments.
- Key Visuals: Average Customer Ratings by Vehicle Type.
- Insight: Determines which vehicle types generate the most mileage and identifies segments where customer satisfaction is highest or needs improvement.
<img width="1144" height="642" alt="Dashboard - 2" src="https://github.com/user-attachments/assets/7113bdef-021a-4f3b-b6d1-9edd37243bff" />

#### 3. Dashboard-3: Revenue & Customer Value:
- Focus: Understanding financial contribution and identifying high-value customers.
- Key Visuals: Revenue by Payment Method (Bar Chart), Top 5 Customers by Total Booking Value (Table), Ride Distance Distribution Per Day.
- Insight: Highlights the contribution of various payment channels (e.g., UPI, Wallet, Cash) to total revenue and allows for the targeting of high-value customers with loyalty programs.
<img width="1131" height="646" alt="Dashboard - 3" src="https://github.com/user-attachments/assets/9831a68e-a0eb-45cf-8759-5fc40d30f8d4" />

#### 4. Dashboard-4: Cancellation Analysis:
- Focus: Detailed investigation into the causes of trip abandonment.
- Key Visuals: Cancelled Rides Reasons (Customer) and Cancelled Rides Reasons (Driver) (Bar Charts).
- Insight: Provides a clear separation and prioritization of friction points.
- For example: quantifying the impact of "Driver asked to cancel" helps management intervene with targeted driver training or policy changes.
<img width="1131" height="645" alt="Dashboard - 4" src="https://github.com/user-attachments/assets/414d66d5-f4cf-4e8e-b9d4-89db52cf468c" />

#### 5. Dashboard-5: Ratings:
- Focus: Evaluating service quality from both the customer and service provider viewpoints.
- Key Visuals:Customer vs. Driver Ratings (Comparison Chart).
- Insight: Ensures a balanced view of service satisfaction and helps isolate discrepancies between customer expectations and driver performance metrics.
<img width="1139" height="649" alt="Dashboard - 5" src="https://github.com/user-attachments/assets/59f8e07d-ce28-4cee-99ef-9d5a1eca677d" />

















