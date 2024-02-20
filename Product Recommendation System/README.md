# Introduction
In today's tech era, online shopping offers convenience, comparison, and access to reviews. To improve personalized offer predictions, the project aims to select the best deals. KNIME, an open-source tool, is chosen for its advanced analytics and machine learning capabilities, covering common data wrangling techniques and allowing for customization.


# Task List
- Data Preparation: Using Row Filter to remove missing data, using String Manipulation to remove special and unrelated characters, then using String to Number to convert data type from String to Numbers.

- Data Visulization: 
  - Top 10 most popular brands/manufacturers and their mean rating: using GroupBy to calculate the total rating and mean rating, then grouping them by manufacturer. Then, I used Sorter and Row Filter to get the 10 most popular brands to do the bar chart visualization. 
  - Top products with the most/least discount price: using Java Snippet to calculate the difference between discount_price and actual_price. Then, continue using Sorter and Row Filter to get the most/least discounted products to create the bar chart visualization. 

- Data model/algortithm: Content-based methodology. 
    Using 3-grams for string similarity analysis, the model recommends products based on user_input in the order of manufacturer, main category, name, price gap, and popularity (no_of_rating). Input is converted to lowercase for consistency. Similarity scores are computed for manufacturer, main category, and name using String Similarity. Price gap percentage and sum of similarity scores are calculated, filtering out items with accuracy > 80%. Recommendations are further sorted by price gap and popularity, with extraneous columns removed for clarity.


# Results: (updating)
