According to that work sheet 
https://lnkd.in/eNg98P5z

I recently analyzed our pizza sales data using Excel pivot tables, and it helped answer some key operational questions. Here’s a breakdown of what I did and how it led to real insights:
📅 1. What days and times do we tend to be busiest?

✅ Step 1: I created two new columns in the worksheet:
Day of Week (extracted from order date)
✅ Step 2: I built a pivot table using:
Rows: Day of Week
Values: Count of Order ID
💡 This instantly showed which days had the most orders. I did the same with Time Buckets to identify peak hours which is Friday .
✅ Step 3: Create a “Time Buckets” Column
To group orders into hour-long slots (like 1pm–2pm), I created a new column called Time Buckets.
Since order times are in exact timestamps (e.g., 01:00:00- 02:00:00 - 1am-2am), I used a VLOOKUP to match each time to a predefined range.
🔥 Key Insight:
Our peak periods are between 12pm–2pm, with a noticeable spike during lunch hours.
 Knowing this helps us plan staffing, kitchen prep, and even promotional timing more effectively.

📅 How many pizzas are we making during peak periods?
✅ Step 1: Add a “Month of the Year” Column
✅ Step 2: Build a Pivot Table
Rows: Month of the Year
Values: Count of Order ID
This showed how many total orders were placed each month, which I used as a proxy for how many pizzas we’re making during those times.
📈 Insight:
July stood out as our busiest month of the year by a clear margin.
This tells us that peak production and demand happen in mid-summer — likely driven by holidays, tourism, or seasonal behavior. That insight helps us:
Plan staffing and inventory better
Launch promotions when they’ll have the biggest impact
Prepare the kitchen for high-volume periods
📅 What are our best and worst-selling pizzas?
 ✅ step 1:create a pivot table 
rows: Pizza_id
value: sum of order_id 
Using a pivot table to analyze our sales data, I evaluated the performance of each pizza by summarizing the total number of orders per pizza ID
📅 What's our average order value?
 ✅ step 1:create a pivot table to get the average of summarize the total price 
📅 How well are we utilizing our seating capacity? (we have 15 tables and 60 seats)
Even during your busiest hour (12–1pm), you're filling only about 31% of your seats on average. That suggests:
Time Slot | Total Pizzas | Avg. Per Day (365 days) | Est. Utilization
12pm–1pm  |   6,772      | ~18.6                   | ~31%
1pm–2pm   | 6,421        | ~17.6                   | ~29%
6pm–7pm   | 5,420        | ~14.8                   | ~25%
5pm–6pm   |  5,211       | ~14.3                   | ~24%
7pm–8pm   | 4,407        | ~12.1                    | ~20%
Even during your busiest hour (12–1pm), you're filling only about 31% of your seats on average. That suggests:
You have room to grow without needing more tables/seats.
There may be opportunities to promote off-peak hours.
Improving table turnover or larger group seating might help boost revenue.



