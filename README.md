# Macros-of-High-Protein-Foods

I'm passionate about fitness alongside data analysis and coding. When it comes to working out, maintaining a balanced diet with sufficient protein is crucial for muscle recovery and growth. I'm curious to explore which foods are the richest in protein and discover any unexpected sources that could enhance my diet and workout performance.

## Data Source

I looked on Kaggle to find any data sources that could help answer my question. The data source I found here https://www.kaggle.com/datasets/fydrose/macros-of-popular-high-protein-foods?select=macros_dataset.csv

## Content
The dataset was pretty new being published around November. The author obtained the data through cross-referencing blogs and lists for high protein foods and then finding the macro content or Fats, Protein, and Carb content of a 100g serving of each food. The dataset contains 60 rows and 8 different attributes. The author categorized each food in a certain food group in the category_name attribute. The origin column describes whther the food came from an animal or not. The diet_type column describes what foods are suitable for the three different types of diets which are Omnivorous, Vegetarian and Vegan.

## Attributes in dataset

* food_name
* proteins_100g
* carbohydrates_100g
* fat_100g
* energy_100g
* category_name
* origin
* diet_type

## Questions

1. General trends macros of high protein foods?
2. Which foods have the highest protein to calorie ratio?
3. Are there any significant difference between Macros and Calories between Diet Types?
4. Which food Groups have the lowest calorie content?

## Data Cleaning
In my data cleaning process using Excel, I noticed that the dataset was already quite clean with no missing values. However, upon examining the category_name column, I realized that some food items were classified too specifically. For instance, there were only a few yogurt items and several milk items, which I felt could be categorized more broadly. I decided to group certain foods that seemed overly specific into more general categories like Legumes, Dairy, and Seafood.
Additionally, I wanted to include a new diet type, Pescatarian, so I identified foods categorized as Seafood and updated their diet types accordingly.

## Data Transformation
I then downloaded the dataset into a CSV file and used the Data Script found in the repository that uploads the data into my local PostgreSQL database. I then used PGAdmin 4 a management tool for PostgreSQL to transform my data and find answers to the questions above. 

## Visualization 
I used PowerBI in order to visualize my data. You can find these Visualizations in the Visualization folder where you can view the powerbi file to interact with the data or just view the pdf file if you want the general gist of it.

## Files in Repository
1. Report Generalization of the Analysis.
2. Visualizations PowerBi Report and Pdf files
3. CSV_To_PSQL_Table.py Script to convert CSV file from Kaggle to local PostgreSQL database
4. Insights Findings from the data.
5. Queries.sql The queries that were done to transform the data to obtain answers to the questions and make creating visualizations on powerbi easier
