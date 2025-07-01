
# 🍕 Pizza Sales Analysis Using Excel Pivot Tables

This project explores a pizza restaurant's sales performance using **Excel pivot tables**. The goal is to uncover operational insights that can help improve staffing, inventory, and overall efficiency.

🔗 **Worksheet Source:** [Pizza Sales Excel File](https://lnkd.in/eNg98P5z)

---

## 📅 When Are We Busiest?

### ✅ Step 1: Extract Day of the Week

* Created a new column to extract the **day of the week** from the `order_date`					
### ✅ Step 2: Analyze Order Volume by Day

* Built a pivot table with:

  * **Rows:** Day of the Week
  * **Values:** Count of `order_id`
* This revealed which days have the highest order counts.
  ## The answer question 1 depends on my analysis=>  Friday is the most day that people visit the resturant, in other word Friday is the busiest day in the week
  ![month](https://github.com/user-attachments/assets/2487fa6a-48f8-43af-8103-ddfdd61b81bc)
### ✅ Step 3: Group Order Times into Time Buckets to get the bussiest time 

* Created a `Time Buckets` column to group timestamps (e.g., 1:00 PM – 2:00 PM).
* Used `VLOOKUP` to assign each order to a specific time range.

### 🔥 Key Insight:

The busiest period is between **12 PM – 2 PM**, with the highest order volume on **Fridays**.

![time](https://github.com/user-attachments/assets/a81e9b9f-39fa-4698-a50c-448fc8b4e8ad)

> This insight supports smarter **staff scheduling**, **kitchen prep planning**, and **promotion timing**.


---

## 📈 How Many Pizzas Are We Making During Peak Periods?

### ✅ Step 1: Add “Month of the Year” Column

* Extracted the month from each order date.

### ✅ Step 2: Monthly Order Volume Analysis

* Built a pivot table with:

  * **Rows:** Month
  * **Values:** Count of `order_id`

### 📊 Insight:

**July** is the busiest month by a significant margin — likely due to **seasonal demand, holidays, or tourism**.

 ![montht](https://github.com/user-attachments/assets/09644a06-b102-48fb-841d-3379c3d8e5e5)

This allows for better **inventory management** and **campaign planning** during peak months.

---

## 🍕 What Are Our Best & Worst-Selling Pizzas?

### ✅ Step: Analyze Orders by Pizza Type

* Created a pivot table:

  * **Rows:** `pizza_id`
  * **Values:** Sum of `order_id`

### 📌 Insight:
		
#### The best = big_meet_s		
#### The worest = the_greek_xxl		
![pizza type](https://github.com/user-attachments/assets/4283fd4c-e5b2-460a-b3fb-2418aa2d4173)

> Identifying top and bottom sellers helps optimize the **menu**, reduce **waste**, and improve **profit margins**.
notes: this screen shot does not get all the values 
---

## 💰 What’s the Average Order Value?

### ✅ Step: Calculate AOV Using Pivot Table

* Built a pivot table to summarize the **average total price per order**.

### 📌 Insight:
![avg](https://github.com/user-attachments/assets/dbd04d16-786c-4f1c-b2ed-36dcf4f6e0af)

> Tracking AOV helps monitor **customer spending patterns** and test the impact of upselling or bundling strategies.

---

## 🪑 How Well Are We Utilizing Our Seating Capacity?

> **Total Capacity:** 15 tables, 60 seats

Using order volume during each time bucket, we estimated average **seating utilization**:

| Time Slot | Total Pizzas | Avg. Per Day | Est. Utilization |
| --------- | ------------ | ------------ | ---------------- |
| 12pm–1pm  | 6,772        | \~18.6       | \~31%            |
| 1pm–2pm   | 6,421        | \~17.6       | \~29%            |
| 6pm–7pm   | 5,420        | \~14.8       | \~25%            |
| 5pm–6pm   | 5,211        | \~14.3       | \~24%            |
| 7pm–8pm   | 4,407        | \~12.1       | \~20%            |

### 📌 Key Insight:

Even during peak lunch hours, only about **31%** of available seats are being used.

#### 💡 Implications:

* There's significant **room for growth** without needing additional space.
* Opportunity to boost revenue through:

  * **Off-peak promotions**
  * **Improving table turnover**
  * **Attracting larger groups**

---

## ✅ Summary

This Excel-based analysis delivered actionable insights for:

* **Optimizing labor and inventory**
* **Improving menu performance**
* **Maximizing space utilization**
* **Driving revenue through targeted strategies**
![dashboard](https://github.com/user-attachments/assets/ba3c90f9-0cd3-4a55-ab91-f02536cadae2)



