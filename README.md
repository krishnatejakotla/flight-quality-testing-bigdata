# ✈️ Flight Quality Testing using PySpark

This project demonstrates end-to-end data validation and quality testing on flight-related datasets using **PySpark**, covering real-world data quality KPIs such as cancellations, delays, and review accuracy.

---

## 📌 Objective

The goal is to simulate a Big Data quality testing scenario by:
- Validating flight data consistency
- Identifying data quality issues
- Testing key performance indicators (KPIs)
- Asserting business rules (e.g., rating scales, delay thresholds)

---

## 🧾 Datasets Used

1. **customer_booking.csv** – Includes passenger counts, trip types, and booking details  
2. **flights_sample_3m.csv** – Contains flight details like origin, destination, delay info  
3. **airlines_reviews.csv** – Passenger reviews and ratings

---

## 🛠 Technologies Used

- **PySpark (Spark SQL & DataFrames)**
- **Google Colab**
- **Pandas**
- **CSV Export for Dashboard Compatibility**

---

## ✅ Key Steps Performed

### 1. Data Quality Checks
- Checked for **nulls**, **duplicates**, and **data types**
- Displayed schemas of all datasets to validate structure

### 2. KPI Calculations
- **Cancellation Rate:** % of flights cancelled by route  
- **Average Departure Delay:** Top 10 delayed routes  
- **Passenger Occupancy Rate:** Ratio of passengers to available seats  
- **On-Time Performance:** Count of timely flights (departure delay = 0)

### 3. Review QA Testing
- Extracted average ratings from reviews
- Asserted all ratings are **≤ 10** (validation rule)
- Exported data for dashboard creation

### 4. Data Exports
- `review_kpis.csv` – Validated average ratings  
- `on_time_kpi.csv` – Cleaned data for on-time metrics  

---

## 📈 Output Sample (KPIs)

| Metric                  | Description                          |
|-------------------------|--------------------------------------|
| `avg_departure_delay`   | Avg delay by route (top 10)          |
| `cancellation_rate`     | % of cancellations per route         |
| `occupancy_rate`        | Booking density by flight            |
| `avg_rating`            | Passenger review rating (scale 0–10) |

---

## 📂 Project Files

- `flight_quality_testing.ipynb` – Main notebook with all code
- `review_kpis.csv` – Output of validated average ratings
- `on_time_kpi.csv` – Clean on-time KPI export

---

## 📌 Highlights

- Focused on **data integrity**, **KPI validation**, and **assertion-based testing**
- Used PySpark's distributed computing features for large dataset handling
- Validated against **realistic rules** used in data quality engineering

---

## 🧑‍💻 Author

**Krishna Teja Reddy Kotla**  
📫 GitHub: [krishnatejakotla](https://github.com/krishnatejakotla)  
📎 Email: [krishnatejareddy.kotla@gmail.com]  

---

## 🗂️ Dependencies

```txt
pyspark
pandas
