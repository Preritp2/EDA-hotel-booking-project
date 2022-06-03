# EDA-hotel-booking-project
project on Hotel Booking Analysis
Abstract: 
Online hotel booking is the latest breakthrough in the hospitality industry. This project contains the real-world data record of hotel bookings of a city and a resort hotel containing details like as when the booking was made, length of stay, the number of adults, children, cancellations, guest details and the number of available parking spaces, etc. Main aim of the project is to understand and visualize dataset from hotel and customer point of view i.e.

•	reasons for booking cancellations across various parameters

•	best time to book hotel

•	peak season

•	guests from different countries

•	market segment and give suggestions to reduce these cancellations and increase revenue of hotels.

Keywords: EDA, Data Analysis, NumPy, pandas, matplotlib, seaborne, Data visualization, Booking & Cancelation.

1.Problem Statement

This project contains the real-world data record of hotel bookings of a city and a resort hotel which helps consumers to book the hotels online. It basically checks the data in every aspect for consumer and makes it easy for them to use. If faces any issues or error occurs will check it accordingly and give the result. 
The main objective is to build a predictive model, which could help in predicting and analysis good hotels. This would in turn help consumers in matching the right hotels quickly and efficiently.

●	hotel: Types of Hotels: Resort Hotel, City Hotel

●	is_canceled: Value indicates booking was canceled (1) or not (0)

●	lead_time: Number of days between the booking date and the arrival date

●	arrival_date_year: Year of arrival date

●	arrival_date_month: Month of arrival date

●	arrival_date_week_number: Week number of year for arrival date

●	stays_in_weekend_nights: Number of weekend nights (Saturday or Sunday) the guest stayed or        booked to stay at the hotel 

●	arrival_date_day_of_month: Day of arrival date

●	stays_in_week_nights: Number of weeknights (Monday to Friday) the guest stayed or booked to      stay at the hotel

●	adults: Number of adults: 

●	children: Number of children

●	babies: Number of babies

●	meal: Type of meal booked. Categories are presented in standard hospitality meal packages: Undefined/SC – no meal package; BB – Bed & Breakfast; HB – Half board 
(breakfast and one other meal – usually dinner); FB – Full board (breakfast, lunch, and dinner)

●	country: Country of origin.

●	market_segment: Market segment categories, “TA” :“Travel Agents” , “TO” : “Tour Operators”, Aviation, Complementary, Corporate, Direct, Groups.

●	distribution_channel: Booking distribution channel. The term “TA” means “Travel Agents” and “TO” means “Tour Operators”, Corporate, Direct.

●	direct is_repeated_guest: Value indicates if the booking name was from a repeated guest (1) or not (0).

●	previous_cancellations: Number of previous bookings that were canceled by the customer prior to the current booking.

●	previous_bookings_not_canceled: Number of previous bookings not canceled by the customer prior to the current booking.

●	reserved_room_type : Code of room type reserved (A,B,C,D,E,F,G,H).

●	assigned_room_type : Code for the type of room assigned to the booking (A,B,C,D,E,F,G,H,I,J,K).

●	booking_changes: Number of changes made to the booking from the moment the booking was entered until check-in or cancellation.

●	deposit_type: This variable has categories: No Deposit – no deposit was made; Non-Refund – a deposit was made in the value of the total stay cost; Refundable – a 
deposit was made with a value under the total cost of the stay.

●	agent: ID of the travel agency that made the booking.

●	company: ID of the company that made the booking or is responsible for paying the booking.

●	days_in_waiting_list: Number of days the booking was in the waiting list before it was confirmed.

●	customer_type: Types  of customer four categories: Contract - when the booking has an allotment or other type of contract associated with it; Group – when the booking is associated to a group; Transient – when the booking is not part of a group or contract and is not associated to other transient bookings; Transient-party – when the booking is transient but is associated to at least other transient bookings

●	adr: Average Daily Rate as defined by dividing the sum of all lodging transactions by the total number of staying nights.

●	required_car_parking_spaces: Number of car parking spaces required by the customer.

●	total_of_special_requests: Number of special requests made by the customer.

●	reservation_status: Reservation status contains three categories: Canceled – booking was canceled by the customer; Check-Out – customer has checked in but already departed; No-Show – the customer did not check in and didn’t inform the hotel its the reason.

●	reservation_status_date: Date at which the last status was set.

2. Introduction

Hotel industry is a very volatile industry and the bookings depend on variety of factors such as type of hotels, seasonality, days of week and many more. Hospitality industry is big contributor to economic growth of any country. This makes analyzing the patterns available in the past data more important to help the hotels plan better. Using the historical data, hotels can perform various campaigns to boost the business. We can use the patterns to predict the future bookings using time series or decision trees. The growth in the hospitality sector and its contributions to the GDP will continue to be substantially increase. But when it comes to booking cancellations, it has a negative impact on it. To reduce and anticipate an increase in the number of booking cancellations, we developed an EDA- Hotel Booking Analysis model which predicts for hotels and give suggestions to reduce these cancellations and increase revenue of hotels. These results can also help hotel owners or hotel managers to predict better predictions, improve cancellation regulations, and create new tactics in business. We will perform exploratory data analysis with python to get insight from the data. All personally identifying information has been removed from the data.

3. Data Cleaning

Checking missing values:

First step will be to clean data; any irrelevant or missing information i.e. NULL values will be removed from the data, so that we can start working on the relevant data.

Here is the total count of null values present in each dataset field. There are total 32 columns.

 



Most of the null values are present in columns: company and agent.

Let’s drop columns with high missing values.

 
Now after drop columns with high missing values the count of columns is 30. 

4. Exploratory Data Analysis
EDA or exploratory data analysis is a technique for fitting linear and higher functions to relationships, for structuring and transforming variables with arithmetic functions, for splitting relationships into partitions and clusters, for extracting features through statistical results and such. One example of the results of EDA is a simple histogram that describes discrete and continuous variables, schematic plots that provide general & partial relationship characteristics that distinguish 2 habits, simplification of functions from low dimensional relationships and two-way tables such as contingency tables. On this part, we would like to visualize some features and show statistical relationship with target variable. This analysis will help to get overall view and deep familiarity of the data, detect extreme values and identify
obvious errors.

Based on this we find some questions which is important to be discussed, as follows., 

●	What is the booking ratio between Resort Hotel and City Hotel?

●	How many bookings were canceled in total and at hotel level?

●	From which country majority of guest came?

●	Which are the busiest months for hotel?

●	In which years maximum bookings are done for both hotels?

●	Which was the most booked accommodation type (Single, Couple, Family)?

●	What are the market segments of both hotels ?

Let’s analyze each question one by one.,


1. What is the booking ratio between Resort Hotel and City Hotel?
 
We can see that the percentage of City hotels is more compared to Resort hotels in terms of bookings.

2. How many bookings were canceled in total?
According to the bar chart, 74745 bookings were not cancelled 44153 bookings were cancelled from both hotels.
3. From which country majority of guest came? 

 
More visitors are from Western Europe, namely Portugal being the Highest, followed by Great Britain (UK), and France.

4. Which are the busiest months for hotel?
Most bookings were done in the month of August, July, May and June.

5. In which years maximum bookings are done for both hotels?
 
47% of bookings were done in the year 2016, then 34% in 2017 and 18% in 2015. 
We can see the increasing tendency in bookings year wisely.

6. Which was the most booked accommodation type (Single, Couple, Family)?
  
The highly booked Accommodations was for Couple, then Single and Family/Friends.

7. What are the market segments of both hotels?
 
Majority of Market segments is Travel agencies(offline/online)s

5. Steps involved:

Null values Treatment:
Our dataset contains a large number of null values which might tend to disturb our accuracy hence we dropped them at the beginning of our project inorder to get a better result.
Exploratory Data Analysis: 
After loading the dataset, we performed this method by comparing our target variable with other independent variables. This process helped us figuring out various aspects and relationships among the target and the independent variables. It gave us a better idea of which feature behaves in which manner compared to the target variable,
6. Results and Discussion:-

These studies confirm that bookings with a high risk of being cancelled can be detected. This encourages hotel management to take steps to deter possible cancellations, such as improved facilities, discounts or other
incentives, from being provided. However, since others are oblivious to this sort of bid, this should not be extended to all consumers. However, this prediction model has much to be learned from building and deploying it.

7. Conclusion:

That's it! We reached the end of our exercise.
Starting with loading the data so far, we have done null values treatment, EDA, data visualization, and then results.
This study aims to explore some of the functions of predictive analytics in scientific analysis from a scientific point of view, including defining which features lead to predicting the likelihood of booking more hotels and reducing cancellations. The implementation of data visualization and data analytics techniques, made it possible to recognize the predictive significance of a feature. Different features were found to vary in value depending on the hotel, and certain features for some of the hotels are not needed. City hotel were booked in majority. So its good to spend the most targeting fund on these hotel. Cancellation ratio of city hotel is high then resort hotel though city hotels bookings are also high comparatively resort hotels. Many guests come from Western European countries. So hotels should spend a significant amount of budget in these areas. May to August are the busiest months so the hotels should target more customers in this period and try to do more business for profit. Most customers are couples and bringing kids along with them is rare so the hotels should advertise in such a way that it attracts the couples more. In Market segment many of the hotel bookings are done from Travel agencies (online and offline). Encourage Direct bookings by offering special discounts. Hotel has low repeated guest; Hotel should depend on online marketing companies for advertising to increase the repeated guests. New Guests cancels the most then the repeated guests. In food most popular meal plan was BB (Bed & Breakfast) preferred by guests.

References-
1.	Almabetter
2.	Geeks for Geeks
3.	Analytics vidhya
