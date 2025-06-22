🚕 Namma Yatri Trip Analysis Dashboard (SQL + Power BI)
This project presents an interactive data analysis dashboard built using SQL and Power BI to explore ride data from Namma Yatri, a Bengaluru-based mobility platform. The goal was to uncover insights into trip volume, customer engagement, and driver performance across different assemblies. Using SQL, raw data was cleaned, transformed, and used to compute KPIs such as total trips, earnings, and conversion rates. Power BI was utilized to visualize these metrics through dynamic charts, trend lines, and maps. The dashboard helps stakeholders make data-driven decisions by highlighting high-demand zones, fare trends, and ride patterns across the city.

Screenshot 2025-04-18 115526

📊 Key Dashboard Insights
🔷 High-Level KPIs:

Completed Trips: 894

Total Searches: 1,980

Estimates Given: 1,612

Quotes Shared: 1,167

Driver Earnings: ₹687K

Conversion Rate: 2.21%

🔷 Visual Analytics:

Trips vs Duration: Trend line highlighting demand fluctuations over time.

Fare vs Duration: Helps evaluate fare distribution over trip lengths.

Distance vs Duration: Identifies efficient vs. inefficient trip durations.

Assembly-wise Searches: Tabular breakdown of ride demand per assembly (e.g., Ramanagaram, Yelahanka).

Map Visualization: Geographic distribution of ride activity across Bengaluru.

🛠️ Tech Stack
🔷 SQL (MySQL/PostgreSQL):

= Cleaned and prepared raw ride data using CTEs, JOINS, aggregation, and date-time functions.

Generated KPIs like ride counts, conversion rates, and driver earnings.
# Total Trips
select count(distinct tripid) from trips_details4;

# Total Drivers
select count(distinct driverid) from trips;

# Total Earning
select sum(trips.fare) from trips;

# Total Complete Trips
select sum(trips_details4.end_ride) Total_Completed_Trips from trips_details4;

# Total Searches
select sum(trips_details4.searches) from trips_details4; -- 2161

# Total Searches which got estimate
select sum(trips_details4.searches_got_estimate) from trips_details4; -- 1758

# Total Searches which for quotes
select sum(trips_details4.searches_for_quotes) from trips_details4; -- 1455

# Total Searches which got quotes
select sum(trips_details4.searches_got_quotes) from trips_details4; -- 1277

# Total Trips cancel by Drivers
select sum(driver_not_cancelled) from trips_details4; -- 1140
select count(*) - sum(driver_not_cancelled) driver_cancelled from trips_details4; -- 1021

# Total Trips cancel by Customers
select sum(trips_details4.customer_not_cancelled) from trips_details4; -- 1120
select count(*) - sum(customer_not_cancelled) customers_cancelled from trips_details4; -- 1041

# Total OTP Enter
select sum(otp_entered) from trips_details4; -- 983

# Total end ride
select sum(end_ride) from trips_details4; -- 983

# Average Distance per Trips
select round(avg(trips.distance), 2) Avg_Distance from trips; -- 14.39

# Average fare per Trips
select round(avg(trips.fare) / count(*), 2) Avg_Fare from trips; -- 0.78

# Distance Travelled
select sum(trips.distance) from trips; -- 14148

# Most Payment Method
select a.method Payment_Method from payment a inner join (select trips.faremethod FareMethod, count(distinct tripid) ID from trips group by trips.faremethod order by count (distinct tripid) desc
limit 1) b on a.id = b.FareMethod;

# Highest payment was made through which instrument
select trips.faremethod, sum(trips.fare) from trips group by faremethod order by sum(fare) desc limit 1; -- 197941

select a.method
from payment a inner join (select trips.faremethod, sum(trips.fare) from trips group by faremethod order by sum(fare) desc limit 1) b on a.id = b.faremethod;

# which two locations had the most trips
select trips.loc_from, trips.loc_to, count(distinct tripid) ID from trips group by loc_from, loc_to order by count (distinct tripid) desc limit 2;


# Top 5 Earning Drivers
select trips.driverid, sum(fare) from trips group by driverid order by sum(fare) desc limit 5;


# Which Duration had more Trips
select duration, count(distinct trips.tripid) as ID from trips group by duration order by ID desc limit 1;

# Which driver , customer pair had more orders
select trips.driverid, trips.custid, count(distinct trips.tripid) PAIR from trips group by driverid, custid order by PAIR desc LIMIT 2;

# search to estimate rate
select round(sum(searches_got_estimate) / sum(trips_details4.searches) * 100, 2) as EST_RATE from trips_details4; -- 81.35

# Area got highest trips in which duration
select * from (select *, rank() over (partition by loc_from order by AB desc) rnk from (select trips.duration, trips.loc_from, count(distinct trips.tripid) as AB from trips group by duration,loc_from) a) c where rnk = 1;

# Area got the highest fares
select * from (select *, rank() over(order by fare desc) rnk from (select trips.loc_from, sum(trips.fare) fare from trips group by loc_from)a)b where rnk=1;

# Area got the Cancellations
select * from (select *, rank() over(order by cancel desc) rnk from (select loc_from, count(*) - sum(driver_not_cancelled) cancel from trips_details4 group by loc_from)a)b where rnk=1;

# Area got the Cancellations
select * from select *, rank() over(order by cus_cancel desc) rnk from (select loc_from, count(*) - sum(customer_not_cancelled) cus_cancel from trips_details4 group by loc_from)a)b where rnk=1;

# Duration got the highest trips and fares
select * from (select *, rank() over(order by AB desc) rnk from (select duration, count(distinct tripid) AB  from trips group by duration)a)b where rnk=1;
🔷 Power BI:

Built an interactive and intuitive dashboard.

Included slicers and filters for assembly selection.

Embedded geospatial maps using Bing Maps integration.

🔷 Dashboard Design

Created a custom canvas background for the dashboard using Figma.

✅ Use Cases
For Operations Teams: Identify high-demand zones and optimize driver allocation.

For Product/Strategy Teams: Track user engagement and booking behavior.

For Policy Makers: Understand urban mobility trends at the assembly level.

🚀 Future Scope
Real-time data integration via APIs.

Predictive modeling for ride demand.

Deployment to Power BI Service with automated refresh.
