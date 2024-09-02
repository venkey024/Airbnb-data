# Airbnb-data

## The Problem Statement :- 

*In the competitive landscape of Airbnb rentals, potential customers often struggle to find suitable accommodations that meet their preferences for pricing, availability, and location.Simultaneously, property owners and managers need insights into market trends to optimize their pricing strategies and improve their listings' attractiveness.*

*This project seeks to address these challenges By performing comprehensive data cleaning, developing interactive geospatial visualizations, and creating dynamic plots, the project aims to provide actionable insights that will help customers find accommodations that fit their standards and assist property owners in making data-driven decisions to enhance their offerings*

### Step - 1 :- Importing File

Just we are importing and read the Json file and converting it into csv for clear understanding

### Step 2:- Data Cleaning and Manipulation

**2.1 Inspecting the Data**

Initially, we inspect the data to understand its structure and the type of information it contains. This involves using functions like head() and describe() to identify any immediate issues or columns that require further cleaning.

**2.2 Adding Useful Data from Existing Information**

Many columns are unnecessary for analyzing variations in price. We add new columns using the present information. For instance:

⭐city

⭐country

⭐longitude

⭐latitude

⭐availability_365

The extraction of city and other details is challenging because they are stored in string format resembling a dictionary. Therefore, we convert these strings into dictionaries and extract the required values.

### Step 3:- Handling Missing Values

**3.1 Replacing Missing Values**

⭐Columns with less than 5% missing values are handled without significant data loss.

⭐ Replace missing values in bedrooms, bathrooms, and beds with the mode.

⭐Replace missing values in security_deposit, weekly_price, and monthly_price with the average.

### Step 4:- Converting Data Types

Next, we ensure that columns have the appropriate data types to facilitate accurate computations and analyses.

⭐Change bedrooms, bathrooms, and beds to integer type.

⭐ Change weekly_price and monthly_price to integer type.

⭐ Change security_deposit to integer type.

⭐ Convert calendar_last_scraped to datetime.


### step 5:- Data Saving 

Save the Cleaned Data to a CSV File

After cleaning and manipulating the Airbnb data, the next step is to save the cleaned data into a CSV file and load it into Power BI for visualization and analysis. we use the below command

df.to_csv('cleaned_airbnb_data.csv', index=False)

### step 6:- Data Visualization

#### Price Analysis and Visualization: 

Used the cleaned data to analyzed and visualized how prices vary across different locations, property types, and seasons. Created dynamic plots and charts that enable users to explore price trends, outliers, and correlations with other variables.

#### Availability Analysis by Season: 

Analyzed the availability of Airbnb listings based on seasonal variations. Visualized the occupancy rates, booking patterns, and demand fluctuations throughout the year using line charts, bar graphs and donut charts


![image](https://github.com/user-attachments/assets/b045f08a-f67e-4a29-8e80-0157f863d581)


### 📊 Dashboard Overview
This dashboard provides key insights into property pricing trends based on location, property type, and seasonality. It includes three main graphs to help users understand where prices are highest and how they change over time.

### 📈 Graphs Included:
1. Top 5 Cities by Average Price
Type: Bar Graph
Description: Displays the five cities with the highest average property prices. This graph helps users quickly see which cities are the most expensive for property purchases.

2. Top 5 Properties by Average Price
Type: Bar Graph
Description: Shows the five types of properties (e.g., apartments, houses) with the highest average prices. It helps users identify which property types are the most valuable on average.

3. Seasonal Wise Average Price
Type: Bar Graph
Description: Illustrates how average property prices vary by season (spring, summer, fall, winter). This graph helps users understand seasonal trends in property pricing.

----------------------------------------------------------------------------------------------------------------------------------------

![image](https://github.com/user-attachments/assets/427bb07b-1184-4072-8755-56c37efbae2e)

### 📊 Dashboard Overview
This dashboard provides an in-depth look into various property metrics such as bedrooms, bathrooms, beds, prices, and more. It includes three main graphs that offer insights into different aspects of the data.

### Key Metrics:
Cities Analyzed: 516
Property Types: 36
Average Price: 278.77

### 📈 Graphs Included:
1. Sum of Bedrooms, Bathrooms, Beds by Accommodates
Type: Horizontal Bar Chart
Description: This chart shows the total number of bedrooms, bathrooms, and beds for different accommodation sizes. It helps users understand the capacity and type of accommodations available.

2. Sum of Price and Extra People by Property Type
Type: Horizontal Bar Graph
Description: This graph displays the total price and the sum of extra people allowed for each property type. It helps users compare different property types in terms of pricing and capacity for additional guests.

3. Sum of Extra People by Cancellation Policy
Type: Gauge Chart
Description: This gauge chart illustrates the total number of extra people allowed under different cancellation policies. It provides a quick overview of how flexible different property types are with additional guests based on their cancellation policies.

----------------------------------------------------------------------------------------------------------------------------------------
![image](https://github.com/user-attachments/assets/2950f134-34f7-438e-9966-506e4a4ab074)

### 📊 Dashboard Overview
This dashboard provides insights into property pricing, capacity, and location-based trends. It includes three different visualizations to help users understand how prices and policies vary across different properties and locations.

### 📈 Graphs Included:
1. Sum of Price and Extra People by Cancellation Policy
Type: Line Graph
Description: This line graph displays the total sum of property prices and the number of extra people allowed under various cancellation policies. It helps users see trends and relationships between pricing and guest allowances for different cancellation options.

2. Sum of Price by Property Type
Type: Bar Graph
Description: This bar graph shows the total sum of prices for different property types. It helps users compare the overall pricing trends across various property categories, making it easier to identify which types of properties are generally more or less expensive.

3. Average Price by City
Type: Geographical Visualization
Description: This geographical visualization map displays the average property price in different cities. It provides a visual overview of how prices vary by location, helping users understand regional pricing trends and identify high-value or affordable areas.

----------------------------------------------------------------------------------------------------------------------------------------

![image](https://github.com/user-attachments/assets/ea7764ab-117b-4262-a4cb-224abce34281)

### 📊 Dashboard Overview
This dashboard includes a powerful drill-through mechanism to provide detailed insights into various property data.

* Drill-Through Feature : Sum of People by Property Type
Description: This feature allows users to explore the total number of people (guests) accommodated by different property types. By using the drill-through mechanism, users can click on a specific property type to view more detailed information, such as the average price, cancellation policies, or seasonal trends related to that property type.
----------------------------------------------------------------------------------------------------------------------------------------
![image](https://github.com/user-attachments/assets/212340ea-96ce-4f59-8477-9067a6d640c5)
### 📊 Dashboard Overview
This dashboard provides a comprehensive view of various property data to help users analyze and make informed decisions.

Overall Information About Rooms
Type: Table Chart
Description : This table chart provides detailed information about rooms across different properties. It includes key metrics such as the number of bedrooms, bathrooms, beds, and accommodates for each property type. The table format allows for easy comparison and filtering of data, enabling users to quickly identify properties that meet specific criteria.



























