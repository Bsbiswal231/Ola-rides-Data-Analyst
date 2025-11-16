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
###### SQL QUERIES: 
<a href="https://github.com/Bsbiswal231/Ola-rides-Data-Analyst/blob/main/Sql-Queries.pdf"> Sql Queries </a>

















