# Assignment 5.1: Customer Coupon Acceptance
---
# Problem Statement
The objective of this project is to analyze the impact of various factors on the acceptance rate of driving coupons. The dataset includes multiple coupon types, such as Bar, Restaurant (< $20), Coffee House, Restaurant ($20-$50), and Carry Out. The goal is to leverage visualizations and probability distributions to effectively differentiate between customers who accepted a coupon and those who did not across these categories.

# Data Cleaning
To address missing values in the dataset, we replaced them with placeholder values. Next, we examined the correlation matrix to assess the relationships between numeric fields. The matrix indicated a perfect negative correlation of -1 between direction_same and direction_opp, suggesting that they convey opposite values for the same attribute. Consequently, we removed the direction_opp column.

We also identified that the toCoupon_GEQ field represents distance thresholds. For better analytical clarity, we consolidated toCoupon_GEQ5min, toCoupon_GEQ15min, and toCoupon_GEQ25min into three distinct categories: '5-15 min', '15-25 min', and '25+ min' in the same column. The Car column had a substantial amount of missing data, leading to its removal to maintain data integrity.
![image](https://github.com/user-attachments/assets/317ee119-2f96-42b7-97b8-e6fe64f70604)

# Data Analysis
The overall coupon acceptance rate in the dataset is 57%. However, the acceptance rates vary across different coupon types are:

Bar: 40.99%

Carry Out & Take Away: 73.38%

Coffee House: 49.86%

Restaurant (20-50): 44.15%

Restaurant (<20): 70.78%

It is important to note that the dataset does not have an equal distribution of samples for each coupon type. The chart below illustrates the sample distribution across the coupon categories.

![image](https://github.com/user-attachments/assets/a7060494-c0cc-4ff0-8134-4b07f3452848)


# Recommendation:
To establish an effective recommendation strategy, the objective is to ensure that the acceptance rate based on our recommendations exceeds the average acceptance rate for each specific coupon type.

# Analysis Structure:
For each coupon type, we will analyze how acceptance rates vary based on different factors. Following this analysis, we will provide targeted recommendations based on the acceptance rate patterns observed for each coupon category.


# Restaurant (<20)
The overall acceptance rate for the Restaurant (<20) coupon is 70.78%. Encouraging group visits with friends, partners, or kids may increase acceptance rates, as they tend to accept more than those dining alone. There is a noticeable drop in acceptance when the restaurant is more than 25 minutes away, so targeting 5-25 minute distances and focusing on No Urgent Place destinations can further drive acceptance. Promotions should be concentrated during 2 PM and 6 PM, which aligns with lunch and dinner times, increase redemption rates. 1-day expiration period has significatly higer acceptance rate than 2h expiration period coupons. Acceptance rates also tend to be higher when the weather is warm, hot, and sunny . Additionally, occupations such as Protective Service, Construction, Life Physical Social Science, Architecture & Engineering, and Sales & Related exhibit higher acceptance rates and should be prioritized.
![image](https://github.com/user-attachments/assets/498c6e13-43cf-41bb-a06f-62dd2f292497)


# Resraurants (20-50)
The overall acceptance rate for the Restaurant (20-50) coupon is 44.15%. To effectively increase acceptance rates for the Restaurant (20-50) coupon, the strategy should focus on targeting frequent restaurant visitors, as we observe a clear trend in the acceptance rate increasing for people who tend to visit Restaurant (20-50) frequently. Promotions should be concentrated between 10 AM and 2 PM, with a 1-day expiration period. People traveling with their partner are highly likely to visit the restaurant compared to when traveling alone or with others. Healthcare Support, Construction, Office & Administrative Support, and Production Occupations may yield higher acceptance rates. Emphasizing group visits with partners and focusing on No Urgent Place destinations can further optimize acceptance rates. A unique trend for Restaurants (20-50) is that driving distance does not seem to affect the acceptance rate.
![image](https://github.com/user-attachments/assets/74c4d805-5b5e-4cb3-8e3f-ba918c633afd)

# Coffee House
The overall acceptance rate for the Coffee House coupon is 49.86%. The strategy should prioritize younger demographics (below 21), who demonstrate higher acceptance rates. Individuals with Some High School and High School Graduate education show higher acceptance levels, aligning well with the young audience, making them a key segment. Promotions should be concentrated between 10 AM and 2 PM, aligning with common coffee break times. There is a clear trend between the distance of the coffee house and the acceptance rate, so it is important to recommend nearby locations. People are more likely to accept the coupon when heading to No Urgent Place or work. Additionally, occupations such as Healthcare Practitioners, Building & Grounds Cleaning, Transportation & Material Moving, Healthcare Support, and Students show higher acceptance rates and should be prioritized. Optimizing redemption can be achieved by emphasizing groups traveling with friends or partners.
![image](https://github.com/user-attachments/assets/147d3165-b262-49d1-a48e-685c5c58a9b4)



# Carry Out
The overall acceptance rate for the Carry Out & Take Away coupon is 73.38%. To effectively increase acceptance rates, the strategy should focus on targeting older age groups (50+), as they exhibit higher acceptance rates. Promotions should be concentrated between 2 PM and 6 PM and those heading home, aligning with lunch and dinner hours when carry-out orders are more likely. Protective Service, Construction & Extraction, Healthcare Practitioners, Building & Grounds Cleaning, and Food Preparation occupations yield higher acceptance rates. Emphasizing group outings with friends and focusing on customers heading home can further optimize acceptance rates. The Carry Out coupon appears to have a higher acceptance rate compared to other coupons, making it a strong recommendation choice for most situations.
![image](https://github.com/user-attachments/assets/28f75710-3577-42a7-93ee-c4a253c91d94)



# Bar 
The acceptance rate for the Bar coupon stands at 40.99%, but there are clear opportunities to improve it. Targeting younger demographics, particularly during 6 PM to 10 PM and those heading home, when bar visits are more common, could effectively boost coupon usage. Certain occupations, such as Architecture & Engineering, Production, and Life, Physical & Social Science, also show higher acceptance rates and should be prioritized. The coupon acceptance rate is higher when traveling with friends and significantly lower when accompanied by a child. There is also a notable trend indicating that frequent bar-goers are more inclined to use the coupon, making them a key target group. A unique aspect of the bar coupon is that the male audience tends to have a much higher acceptance rate than females.
![image](https://github.com/user-attachments/assets/5fe22ff2-3b56-42a3-adc7-56693ed1f3c7)

# Coupon Acceptance based on Occupation
![image](https://github.com/user-attachments/assets/b32368ed-f624-4d22-8ab9-07ebf17918e5)








