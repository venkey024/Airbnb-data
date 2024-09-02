![image](https://github.com/user-attachments/assets/6df18691-8ff1-4444-8b5f-a87ce2c40c12)# Airbnb-data

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




![image](https://github.com/user-attachments/assets/427bb07b-1184-4072-8755-56c37efbae2e)




![image](https://github.com/user-attachments/assets/b045f08a-f67e-4a29-8e80-0157f863d581)



![image](https://github.com/user-attachments/assets/2950f134-34f7-438e-9966-506e4a4ab074)


![image](https://github.com/user-attachments/assets/ea7764ab-117b-4262-a4cb-224abce34281)





























