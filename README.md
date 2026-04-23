# Analysing Booking trends in the Hospitality Industry

## Business Introduction
A predictive model to determine the booking status of a customer
Hotel haven is a hotel chain with multiple locations. The hotel offers a wide range of services including various types of rooms, meal plans an dparking options.
Hotel Haven has been facing challenges in predicting customer cancellations, which impacts thier ability to manage resources effectively. The hoel wants to better understand their booking patterns and create strategies that could improve customer retention and reduce cancellations.

## Problem Statement 
The hotel struggle swith high cancellation rates, leading to lost revenue and inefficient resource allocation. The existing system doe snot provide sufficient insights into why customers cancel their bookings. The hotel management seeks to predict cancelations based on booking data to improve operational efficiency and customer retention. 

## Rationale for the project
**Understanding Cancellations**
Analysing booking patterns help uncover the underlying reasons why customers cancel their bookings.

**Identifying Key Factors**
By examining variables like lead timer, room type, market segment and price, the project alows the identification of specific factors that influence customers decision to either cancel or keep their bookings.

**Optimising customer satisfaction**
By minimising cancellations, the hotel can ensure better resource allocation and improved guest experience. customers who are less likely to cancel will contribute to smoother operations and increased satisfaction. 

## Deliverables 
- Data Cleaning
- Data Exploration
- Comprehensive Data Analysis
- Feature Engineering and Model Development
- Model Evaluation and Finetuning 
- Jupyter Notebook and Powerpoint Slideis

## Data Dictionary

Booking_ID - Unique identifier for each booking String

number of adults - Number of adults in the booking Integer

number of children - Number of children in the booking Integer

number of weekend nights - Number of weekend nights included in the booking Integer

number of week - nights Number of week nights included in the booking Integer

type of meal - Meal plan selection (e.g., Meal Plan 1, Not Selected) Categorical

car parking space - Whether the booking includes parking (0: No, 1: Yes) Binary

room type -  Type of room booked (e.g., Room_Type 1, Room_Type 2) Categorical
lead time - Time between the reservation and check-in date Integer
market segment type - Booking channel (e.g., Online, Offline) Categorical


repeated - Whether the booking is from a repeat customer (0: No, 1: Yes) Binary
P-C - Customer profile type indicator (0: Not Customer, 1: Customer) Binary

P-not-C - Non-customer profile type indicator (0: Not Non-Customer, 1:
Non-Customer) Binary.

average price - Average price of the booking Float
special requests - Number of special requests made by the customer Integer
date of reservation - Date the reservation was made Date

booking status -  Status of the booking (e.g., Canceled, Not Canceled) Categorical


1.	who were our customers – 
Were they returning or new customers?
Bookings were done by an overwhelming majority from non-Customer profiles. Just 1% of bookings were made from customer profiles
Insert Pie Chart of  P-C
What channel were the bookings from? 
Most of the bookings were done from Online, followed by offline followed by corporate, then complementary and then aviation. 
Insert Bar chart of booking by market segment. 
Did they usually repeat booking or were they new bookings? 
About 35355 were not repeated bookings. Just 930 bookings were repeated bookings. Can I see who repeated by room type and market segment? 
Insert Repeated Bookings graph 
2.	What were their booking pattern preferences?
what did they choose across board. 
meal type – Most bookings were made choosing meal type 1 then meal type 2. Only 5 bookings were made choosing meal type 3. 5132 bookings were made without selecting meal plans. That means most of bookings prefer meals and they preferred meal type 1. 
Insert Meal type Count graph
Room Type - Room Type 1 had the most bookings with 28138 booked followed by Room type 4 with 6059. The least room type booked is Room type 3 with just 7 bookings.
Insert Booking by Room type graph.
Car parking request – Most bookings were made without a car parking space request. Just 1124 bookings were made with a car parking space request. 
Insert Car parking request count graph 
Special Request – The higher number of bookings were made without any special requests (19780) followed by 11379 bookings with 1 special request and 4634 bookings with 2 requests. 676 bookings were made with 3 special requests and 78 bookings with 4 special requests. Just 8 bookings were made with 5 special requests. 
Insert Special request count graph
how long did they book to stay by market segment type, by roomtype, by special request. 
3.	Who cancelled and what reasons made them cancel? ie price, lead time booking, market segment, room type.
how many cancellations did we have? 
Insert Cancellation count graph
show cancellations by room type, 
Room type 1 had the highest cancellations 9076 but also non cancellations 19062, followed by room type 4 with 2069 can cellations but 3990 non cancellations. Room type 6 had 406 cancellations and 560 non cancellations. Room type 2 had 228 cancellations but 464 non cancellations. Room type 5 had 7 cancellations and 193 non cancellations. Room type 7 had 36 cancellations and 122 non cancellations. Room type 3 had 2 cancellations and 5 non cancellations. 
Insert Room type by cancellation chart. 
market segment, 
Online bookings recorded the highest number of cancellations (8,478); however, this is proportional to their overall booking volume (14,743 non-cancellations). In contrast, complementary customers had no cancellations but was the channel with the lowest bookings. The higher cancellations are driven by scale rather than an unusually high cancellation rate.
Insert market segment and cancellation chart
What made them cancel? 
Price? 
We can infact see that room prices for people that cancelled were higher than those who didn’t cancel. From Room types, Room 7 had the highest average price and also the highest cancellation followed by room type 6 then room type 5 then room type 4
This is also true if we look at the average pricing by market segment type. Average prices were higher for the cancelled bookings. 
 Lead time? 
We can see from box plot that higher lead times accounted for more cancellations usually between more than 100 days. Find graph that answers the question of whether higher lead time caused cancellation. 
Insert box plot of lead time 

Longer lead times also contributed to cancellations as the chart shows us. We can see that average lead days for cancelled bookings were also higher than bookings that weren’t cancelled. This is true when you look at both by market segment type and room type with offline bookings accounting for the highest lead days compared to bookings not cancelled in same category. Online bookers also booked in advanced but eventually had high cancellation rates compared to those who didn’t cancel in same category. 

meal plan, 
week or weekend night booking days, 
repeated bookings, 
We can see a correlation plot to further drive home this point and also see how other factors affected the 
4.	Suggestions

We could advertise other room types that weren’t booked that had averagely lower prices. Not sure about this because average prices could be affected by how many nights were booked and who booked them. Matbe some could have booked more expensive rooms for more nights which not lot of people booked. 
