# 🏨 Hotel Booking Cancellation & Demand Analysis

A comprehensive data analysis and predictive exploration project on hotel reservation patterns, guest demographics, and booking cancellation drivers. Developed in Google Colab as a Big Data course project.

**Author:** Sena Adane

---

## 📌 Project Overview

This project analyzes hotel reservation data to uncover key operational insights and guest behavioral patterns. By evaluating factors like lead times, guest demographics, and special requests, the analysis aims to identify primary drivers behind booking cancellations and lay the foundation for predictive forecasting models.

---

## 🗂️ Dataset Description

The dataset covers hotel booking details from resort and city properties. Below are the primary feature categories and variables analyzed within the project:

| Category | Feature Name | Description | Data Type |
| :--- | :--- | :--- | :--- |
| **Target** | `is_canceled` | Cancellation status (1 = Canceled, 0 = Check-in/Completed) | Binary |
| **Hotel Metadata** | `hotel` | Type of hotel (*Resort Hotel* or *City Hotel*) | Categorical |
| | `is_repeated_guest` | Flag indicating if the booking is from a repeat customer | Binary |
| **Time & Schedule** | `lead_time` | Number of days between booking date and arrival date | Integer |
| | `arrival_date_year` | Year of arrival date | Integer |
| | `arrival_date_month` | Month of arrival date | Categorical |
| | `arrival_date_week_number` | Week number of arrival date | Integer |
| | `stays_in_weekend_nights` | Number of weekend nights (Sat/Sun) stayed or booked | Integer |
| | `stays_in_week_nights` | Number of week nights (Mon–Fri) stayed or booked | Integer |
| **Demographics** | `adults` | Number of adults | Integer |
| | `children` | Number of children | Integer |
| | `babies` | Number of babies | Integer |
| | `country` | Country of origin (ISO code) | Categorical |
| | `market_segment` | Market segment designation (e.g., Direct, Corporate, TA/TO) | Categorical |
| **Preferences & Services** | `meal` | Type of meal booked (BB, HB, FB, Undefined/SC) | Categorical |
| | `reserved_room_type` | Code of room type reserved | Categorical |
| | `assigned_room_type` | Code for room type assigned at check-in | Categorical |
| | `required_car_parking_spaces` | Number of car parking spaces requested | Integer |
| | `total_of_special_requests` | Total number of special requests made by the guest | Integer |
| **Booking Adjustments** | `booking_changes` | Number of changes/amendments made to the reservation | Integer |
| | `days_in_waiting_list` | Days the booking remained on the waiting list before confirmation | Integer |
| | `deposit_type` | Indication if deposit was made (No Deposit, Non Refund, Refundable) | Categorical |

---

## 🔍 Core Analysis Questions

The analysis is structured around six core operational dimensions:

### 1. Cancellation Dynamics
* **Overall Rate:** What is the baseline cancellation rate across all reservations?
* **Hotel Variations:** How do cancellation patterns differ between City and Resort hotels?
* **Temporal Trends:** Are there seasonal spikes or yearly trends in cancellation behavior?

### 2. Lead Time Patterns
* **Booking Window:** How far in advance do guests make reservations?
* **Cancellation Correlation:** Does a longer lead time significantly increase the risk of cancellation?
* **Room Type Impact:** Is lead time correlated with specific reserved room categories?

### 3. Guest Demographics & Origin
* **Composition:** What is the typical ratio of adults, children, and babies per reservation?
* **Geographic Distribution:** Which origin countries generate the highest guest volume?

### 4. Booking Behaviors
* **Stay Duration:** How are stays distributed between weekend nights vs. weekday nights?
* **Seasonality:** Which months or weeks observe peak booking activity?

### 5. Preferences & Amenities
* **Meal Plans:** What are the most frequently selected meal packages?
* **Parking Requirements:** How does parking request frequency vary by customer segment?

### 6. Adjustments & Special Requests
* **Request Frequency:** How often do guests submit special requests?
* **Modification Impact:** Do post-booking changes correlate with lower or higher cancellation rates?

---

## 📊 Key Findings & Insights

> *Note: Metrics below summarize the conclusions drawn from the dataset analysis.*

* **Cancellation Rate:** Highlighted key variations across different hotel types and identified seasonal fluctuations in drop-off rates.
* **Lead Time:** Bookings placed significantly further in advance exhibited a higher probability of cancellation compared to short-notice bookings.
* **Demographics:** The majority of reservations consisted of adult travel groups, with primary guest volume concentrated in top origin regions.
* **Stay Patterns:** Clear distinctions emerged between weekend getaway trends and extended weekday stays.

---

## 🔮 Predictive Modeling Goals

Building on the exploratory findings, the dataset supports the following predictive targets:

1. **Cancellation Risk Scoring:** Classify the likelihood of a new booking canceling based on lead time, customer history, and booking modifications.
2. **High-Risk Period Forecasting:** Identify calendar windows prone to elevated cancellations for proactive yield management.
3. **Customer Segmentation:** Forecast behavior and cancellation probability for specific customer tiers and hotel properties.

---
