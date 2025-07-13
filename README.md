# Hotel Data Analysis and Revenue Optimization Project

## Introduction
The project focuses on leveraging data analytics to improve booking management and revenue optimization for a prominent hotel chain. Using Power BI and data analytics, the goal is to develop actionable insights from hotel booking data. This analysis examines patterns in bookings, guest demographics, and operational performance to provide recommendations that will help the hotel enhance customer satisfaction and maximize revenue.

## Problem Statement
The hotel chain faces challenges in managing bookings effectively and optimizing revenue. They are struggling to understand booking patterns, guest preferences, and the underlying reasons for cancellations. The hotel is also seeking to enhance its revenue management strategies and improve operational efficiencies. Data-driven insights are needed to address these issues, optimize resources, and improve the guest experience.

## Data Sourcing
The data used in this analysis was sourced from the hotel's internal booking system and contains detailed information on:  
- **Booking Details**: Including booking dates, room types, and prices.  
- **Guest Demographics**: Information about new versus repeat guests, their preferences, and booking history.  
- **Operational Data**: Including total revenue, average daily rates (ADR), cancellation rates, and booking channels.  

Data was collected over a period spanning from January 2018 to July 2020 to capture a comprehensive view of booking trends and operational performance.

## Data Transformation and Cleaning
The dataset underwent several steps of transformation and cleaning:
- **Data Merging**: Combined multiple data sources (e.g., booking data, guest data, and revenue data) into a unified dataset for analysis.
- **Missing Values**: Missing or incomplete records were addressed through imputation methods or by excluding incomplete rows from analysis.
- **Outliers**: Anomalous booking values and unusually high or low revenue figures were identified and either corrected or excluded.
- **Data Normalization**: Data was normalised to ensure consistency in units (e.g., converting revenue to consistent currency units) and format (e.g., ensuring dates were uniformly formatted).

These steps ensured that the dataset was clean, accurate, and ready for further analysis.

## Data Modeling
In this phase, relationships between various tables were established to build a coherent data model that allows for cross-table analysis. There were one to many relationships between the fact table (the hotel booking table) and other dimension tables (using their primary keys). Key tables and relationships were created in the model, using foreign keys. They include:
- **Fact table**
- **Market segment dimension** (connected with the market segment ID)
- **Meal cost dimension** (connected with the meal cost ID)
- **Date dimension** (connected with the reservation status date)
- **Location dimension** (connected with the country code)
- **Hotel dimension** (connected with the hotel ID)
- **Distribution dimension** (connected with the distribution channel ID)

This structured data model allows for flexible analysis and insights across multiple variables, such as guest types, booking channels, and room performance.

## Data Analysis and Visualisation
The dashboard is built using Power BI to showcase critical insights derived from the data:
- **Booking Trends**: A line chart illustrates peak and off-peak booking trends across the years, with a noticeable decline in 2020 due to the global pandemic.
- **Revenue Breakdown**: The total revenue is broken down by hotel (City Hotel vs. Resort Hotel), showing a significant contribution from the City Hotel.
- **Guest Demographics**: A pie chart visualizes the breakdown of bookings between new and repeat guests, highlighting a strong base of repeat customers.
- **Room Type Performance**: Revenue performance by room type is displayed, identifying room types like ‘A’ generating the highest revenue.
- **Cancellation Rates**: A bar chart details the cancellation rates by distribution channel, with TA/TO (Tour Operators) having the highest cancellation rate at 29.9%.

These visualisations provide actionable insights into key business performance indicators, enabling stakeholders to make data-driven decisions.

## Conclusions and Recommendations
Based on the analysis and visualisation, the following conclusions and recommendations can be made:

### Booking Trends:
- There is a significant peak in bookings during mid-2018 and a sharp decline in 2020, likely due to external factors like the pandemic.
- **Recommendation**: The hotel should plan promotional campaigns during the peak periods and consider strategies for addressing the seasonal decline.

### Revenue Optimization:
- The City Hotel contributes more to revenue than the Resort Hotel, indicating that business travellers may prefer city locations.
- **Recommendation**: Consider investing in marketing and promotions targeted at business travellers to further capitalise on this segment.

### Guest Demographics:
- New guests account for a small portion (3.75%) of the bookings, with repeat guests making up the majority.
- **Recommendation**: Focus on loyalty programs and targeted marketing campaigns to retain existing guests while attracting new ones.

### Cancellation Rates:
- The cancellation rate is highest for bookings made through tour operators (TA/TO) at 29.9%.
- **Recommendation**: Review the booking process for tour operators to identify any friction points, and explore reducing cancellations through flexible policies or better communication.

### Room Type Performance:
- Room type A generates the highest revenue, whereas room types B and C underperform.
- **Recommendation**: Assess the pricing strategy for underperforming room types or consider adjustments to their features and amenities to boost their appeal.
