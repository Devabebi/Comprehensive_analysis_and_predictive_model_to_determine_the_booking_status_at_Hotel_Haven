# Comprehensive_analysis_and_predictive_model_to_determine_the_booking_status_at_Hotel_Haven
This models revealed key drivers such as lead time, room preferences, etc that significantly impacted bookings. Based on these insights, I proposed data-driven strategies to reduce cancellations, improve customer retention, and optimize resource planning. This project demonstrated the power of predictive analytics to influence strategic decisions.
![hotel_haven](https://github.com/user-attachments/assets/612ce092-3ab2-494f-9694-e5ccefb50e92)


## Table of Content
- [Business Overview](#business-overview)
- [Problem Statement](#problem-statement)
- [Project Objectives and Workflow](#project-objectives-and-workflow)
- [Descriptive Statistics](#descriptive-statistics)
- [Average Booking Price Pattern](#average-booking-price-pattern)
- [Meal Plan Patterns](#meal-plan-patterns)
- [Room Type Patterns](#room-type-patterns)
- [Channel Patterns](#channel-patterns)
- [Lead Time](#lead-time)
- [Booking Cancellation Summary](#booking-cancellation-summary)
- [Supervised Machine Learning: Booking Status Prediction](#supervised-machine-learning-booking-status-prediction)
- [Recommendations](#recommendations)


## Business Overview
<img width="860" height="860" alt="image" src="https://github.com/user-attachments/assets/289e74f3-d575-47c2-bed3-c292281248f1" />

Hotel Haven is a luxury hotel chain with multiple locations. They offers a wide range of services, including various types of rooms, meal plans, and parking options. 

Hotel Haven has been facing challenges in predicting customer cancellations, which impacts their ability to manage resources effectively. 


## Problem Statement
<img width="1331" height="933" alt="image" src="https://github.com/user-attachments/assets/864610a8-6c4d-4745-bf8c-2975b2a5f8de" />

The hotel struggles with high cancellation rates, leading to lost revenue and inefficient resource allocation. 

The existing system does not provide sufficient insights into why customers cancel their bookings. 

The hotel wants to better understand their booking patterns and create strategies that could improve customer retention and reduce cancellations.


## Project Objectives and Workflow
<img width="510" height="803" alt="image" src="https://github.com/user-attachments/assets/09f8aefa-508e-4960-8582-ecb1cfc56549" />

- **Data Cleaning**
- **Data Exploration**
- **Comprehensive Data Analysis**
- **Feature Engineering and Model Development**
- **Model Evaluation and Fine Tuning**


## Descriptive Statistics
<img width="2761" height="919" alt="image" src="https://github.com/user-attachments/assets/e34b4958-e608-4d38-8201-4de6b4a2a5b5" />

Most bookings are **couples (2 adults), without children.**
Typical stay: **2–3 nights (1 weekend + 2 weeknights).**
Lead times highly variable  mix of **last-minute and early planners**.
Average price **~$100/night**, but wide spread indicates seasonal/tiered pricing.
Guests make **~1 special request** on average moderate personalisation demand.
**No repeat guests or car parking** captured in the dataset.


## Average Booking Price Pattern
<img width="2973" height="897" alt="image" src="https://github.com/user-attachments/assets/dcf224ae-3368-4985-9022-d418c5ef3e3f" />

Price does not strongly depend on the number of adults, children, or length of stay.
Instead, price is more influenced by season, room type, and promotional activity.

<img width="2824" height="1048" alt="image" src="https://github.com/user-attachments/assets/09697cc0-729f-4599-a7d7-a70bb67d3a12" />

Prices peak in the summer and on Sundays, whilst winter and Thursdays tend to be cheaper.


## Meal Plan Patterns
<img width="1270" height="824" alt="image" src="https://github.com/user-attachments/assets/8b5aeb42-cef5-4a77-957f-34973f350946" />

Meal Plan 1 is by far the most popular, chosen in nearly 80% of bookings.
Meal Plan 2 shows the highest rate of cancellations (around 37%).

<img width="1299" height="742" alt="image" src="https://github.com/user-attachments/assets/e14e17bc-2f88-45d4-a4b6-3615e8ede5f3" />

Customers who did not select a meal plan also cancelled more often.
Meal Plan 3 is rarely chosen, despite its lower price, suggesting it lacks appeal.


## Room Type Patterns
<img width="1941" height="914" alt="image" src="https://github.com/user-attachments/assets/4c1ba5ea-1940-402c-bf0e-ae6b7d791c88" />

Most of the advance bookers included Room Type 2 and Room Type 5 are prone to cancellation.
Room Types 6 stand out with very high cancellation percentages (over 41%), followed by 2, 3, & 4.

<img width="1036" height="933" alt="image" src="https://github.com/user-attachments/assets/eee52988-6182-4ec3-b1b8-157cb6f0a69a" />

Other premium room types (4, 5, 6, 7) are less frequently booked, possibly due to being overpriced or misaligned with customer preferences.


## Channel patterns
<img width="1950" height="897" alt="image" src="https://github.com/user-attachments/assets/4c0cfaff-5810-4343-8107-5f6646ab5270" />

Most of the advance bookings made online and aviation stand higher cancellation chance.
Online channels dominate but are also the most prone to cancellations (around 34%).

<img width="959" height="907" alt="image" src="https://github.com/user-attachments/assets/05745942-35f2-4f6a-862d-b22e15919038" />

Corporate & Offline bookings are much more reliable, with cancellations as low as 9% and 12%.
No cancellation rate recorded for Complementary


## Lead Time
<img width="1865" height="684" alt="image" src="https://github.com/user-attachments/assets/2007e4ba-cfe6-4577-af7d-3e42e40360fe" />

Bookings made 150–200 days in advance are the most unstable, with a high likelihood of cancellation.
Last‑minute bookings, by contrast, are far more reliable.

<img width="1791" height="616" alt="image" src="https://github.com/user-attachments/assets/90b19a96-90da-4620-9650-5258ace4f6f0" />

Guests who plan longer stays do tend to book earlier, though this effect is relatively weak.


## Booking Cancellation Summary
<img width="1184" height="1072" alt="image" src="https://github.com/user-attachments/assets/66878ea8-d78d-4625-834a-8e9a31ce574d" />

The total of 18563 bookings were not cancelled, and overall cancellation rate is about 71%.

The total of 7446 booking were cancelled, and overall cancellation rate is about 29%.

This level of cancellations has a significant effect on forecasting, revenue management, and the allocation of resources.


## Supervised Machine Learning: Booking Status Prediction

- **Using Multiple Classification Model**

<img width="1038" height="622" alt="image" src="https://github.com/user-attachments/assets/773ef87a-ec2e-4c10-a841-baf027042340" />

<img width="1145" height="553" alt="image" src="https://github.com/user-attachments/assets/6b56f840-3dc5-413b-9d01-14ba57fcb58d" />

Random Forest Model has 86% accuracy with balanced precision & recall, strong ability to predict both cancellations and non-cancellations.

- **Using AutoML**
<img width="1193" height="637" alt="image" src="https://github.com/user-attachments/assets/35691c13-c6b6-4686-987f-4a3b57382c4f" />

<img width="1521" height="235" alt="image" src="https://github.com/user-attachments/assets/ea1f6f25-2364-4526-a933-81037badc3a1" />

AutoML has ~85% but predicts nearly all bookings as cancellations, cannot reliably identify guests who will not cancel.
Accuracy, F1 Score, and Confusion Metric are used to select the best performing model.


## Recommendations

- **Cancellation Policy & Booking Terms**
Tiered Cancellation Fees e.g., full refund if cancelled **30+ days before**, partial refund if **within 7 days**.
Apply **non-refundable** deposit to **long lead bookings** (150–200 days ahead).
Flexible options for the last-minutes reservations

- **Pricing & Revenue Management**
Dynamic Pricing.
Weekend & Seasonal Premiums.
Redesign **Meal Plan 2** and either improve **Meal Plan 3** offering or remove.
Review marketing and pricing of **Room Types 2 & 6** and ensure **Room Types 4, 5, 6, and 7** are competitively priced and clearly positioned.

- **Channel Management**
Reduce overdependence on **Online** 
Improve corporate partnership with **Corporate and Aviation** where cancelations are moderate.
Give loyalty points, special discounts, or perks (late check-out, free breakfast) for customers booking directly i.e **Offline**

- **Operation Efficiency**
Use the Random Forest model to flag likely cancellers and send reminders about cancellation terms or incentives (discounts/upgrades) to confirm.
Don’t allocate staff or block rooms for **high-risk bookings** until closer to check-in.
Use demand patterns **(summer peak, winter dip)** to adjust staffing levels.
Carefully overbook based on model predictions to offset expected cancellations
Customer retention via loyalty program to encourage repeat, more stable customers.


## Thank you
Reach out for more info!
<img width="1584" height="396" alt="Python SQL R MachineLearning MySQL DataAnalysis DataVisualization Statistics BigDataAnalysis Pandas NumPy CloudComputing AWS Azure Tableau CommunicationSkills ProblemSolving BusinessIntelligence PostgreSQL" src="https://github.com/user-attachments/assets/02f76644-4217-4908-a344-ec0b6f666923" />
