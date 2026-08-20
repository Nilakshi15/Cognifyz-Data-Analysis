Cognifyz Data Analysis Internship

Overview

This project contains my data analysis work completed as part of the Cognifyz Data Analysis Internship.

The analysis is performed on a restaurant dataset containing 9,551 records and 21 attributes. The project covers exploratory data analysis, restaurant ratings, cuisine analysis, geographic analysis, restaurant chains, reviews, votes, and service availability.

Technologies Used

Python 3.14

Jupyter Notebook

Pandas

NumPy

Matplotlib

Seaborn

Folium

Project Structure

Cognifyz-Data-Analysis/
├── Dataset/
│   └── Dataset.csv
├── Level_1/
│   └── Level_1_Analysis.ipynb
├── Level_2/
│   ├── Level_2_Analysis.ipynb
│   ├── cuisine_combinations.png
│   ├── cuisine_combination_ratings.png
│   ├── restaurant_chains.png
│   └── restaurant_map.html
├── Level_3/
│   ├── Level_3_Analysis.ipynb
│   ├── Task_1_Restaurant_Reviews/
│   ├── Task_2_Votes_Analysis/
│   └── Task_3_Price_Range_Services/
└── README.md

Level 1 — Exploratory Data Analysis

Task 1 — Top Cuisines

Objectives

Identify the most common cuisines.

Calculate their prevalence.

Visualize cuisine popularity.

Conclusion

The analysis identified the three most commonly served cuisines in the dataset: North Indian, Chinese Cuisine, and Fast Food. North Indian was the most prevalent cuisine, followed by Chinese Cuisine and Fast Food.

Task 2 — City Analysis

Objectives

Identify the city with the highest number of restaurants.

Calculate the average restaurant rating for that city.

Visualize the restaurant distribution by city.

Results

City with highest number of restaurants: New Delhi

Number of restaurants: 5,473

Average rating: 2.44

Conclusion

New Delhi has the highest concentration of restaurants in the dataset, with 5,473 restaurants. However, its average rating is 2.44, indicating that a high number of restaurants does not necessarily correspond to higher average ratings.

Task 3 — Price Range Distribution

Objectives

Determine the most common price range.

Calculate the number and percentage of restaurants in each price category.

Visualize the price distribution.

Results

Most common price range: 1

Number of restaurants: 4,444

Percentage: 46.53%

Conclusion

Price Range 1 is the most common category, representing 46.53% of the restaurants. This shows that a large portion of the restaurants in the dataset belong to the lower price category.

Task 4 — Online Delivery

Objectives

Analyze the availability of online delivery.

Compare the number of restaurants with and without online delivery.

Compare average ratings based on online delivery availability.

Results

Online Delivery

Restaurants

Percentage

No

7,100

74.34%

Yes

2,451

25.66%

Average rating without online delivery: 2.47

Average rating with online delivery: 3.25

Conclusion

Most restaurants in the dataset do not provide online delivery. Restaurants offering online delivery have a higher average rating of 3.25 compared with 2.47 for restaurants without online delivery.

Task 5 — Restaurant Ratings

Objectives

Analyze the distribution of aggregate ratings.

Determine the most common rating range.

Calculate the average number of votes received by restaurants.

Results

Rating Range

Restaurant Count

Percentage

0–1

2,148

22.49%

1–2

10

0.10%

2–3

1,891

19.80%

3–4

4,388

45.94%

4–5

1,114

11.66%

Average number of votes: 156.91

Conclusion

The 3–4 rating range is the most common, containing 4,388 restaurants and representing 45.94% of the dataset. The average restaurant receives approximately 156.91 votes.

Level 2 — Advanced Analysis

Task 1 — Restaurant Ratings

Objectives

Analyze the distribution of aggregate ratings.

Determine the most common rating range.

Calculate the average number of votes received by restaurants.

Results

Rating Range

Restaurant Count

Percentage

0–1

2,148

22.49%

1–2

10

0.10%

2–3

1,891

19.80%

3–4

4,388

45.94%

4–5

1,114

11.66%

Most common rating range: 3–4

Restaurants in this range: 4,388

Percentage: 45.94%

Average number of votes: 156.91

Conclusion

The 3–4 rating range is the most common rating category, accounting for 45.94% of restaurants. This indicates that most rated restaurants fall into the moderate-to-good rating range. The average number of votes received by a restaurant is 156.91.

Task 2 — Cuisine Combinations

Objectives

Identify the most common cuisine combinations.

Compare the average ratings of cuisine combinations.

Identify the highest-rated cuisine combination.

Results

Highest-rated cuisine combination: Modern Indian

Average rating: 4.35

Number of restaurants: 11

Conclusion

The analysis shows that cuisine popularity and rating quality are not necessarily the same. Modern Indian achieved the highest average rating of 4.35 among the analyzed cuisine combinations, with 11 restaurants.

Task 3 — Geographic Analysis

Objectives

Analyze restaurant locations using latitude and longitude.

Identify areas with high restaurant concentration.

Create an interactive restaurant map.

Results

An interactive Folium restaurant map was created.

Restaurant locations were visualized using geographic coordinates.

Map file: restaurant_map.html

Conclusion

The geographic analysis shows that restaurants are concentrated in major urban areas. The interactive map provides a visual representation of restaurant locations and helps identify areas with high restaurant density.

Task 4 — Restaurant Chains

Objectives

Identify the most popular restaurant chains.

Determine the number of restaurants belonging to major chains.

Compare restaurant-chain popularity with average ratings.

Identify the highest-rated restaurant chain.

Results

Most popular restaurant chain: Cafe Coffee Day

Number of restaurants: 83

Highest-rated restaurant chain: Barbeque Nation

Average rating: 4.35

Conclusion

Cafe Coffee Day has the largest presence in the dataset with 83 restaurants, while Barbeque Nation has the highest average rating of 4.35. This shows that the most widespread restaurant chain is not necessarily the highest-rated one.

Level 3 — Advanced Analysis

Task 1 — Restaurant Reviews

Objectives

Analyze the text reviews to identify common positive and negative keywords.

Calculate the average length of reviews.

Explore the relationship between review length and rating.

Dataset Limitation

The provided dataset does not contain a dedicated text-review column. Therefore, actual positive/negative keyword extraction, review-length calculation, and review-length versus rating analysis could not be reliably performed.

Instead, the available Rating text column was analyzed.

Results

Rating Text

Percentage

Average

39.13%

Not rated

22.49%

Good

21.99%

Very Good

11.30%

Excellent

3.15%

Poor

1.95%

Conclusion

The Rating text analysis shows that Average is the most common rating category at 39.13%, followed by Not rated at 22.49% and Good at 21.99%. Only 3.15% of restaurants are categorized as Excellent, while 1.95% are categorized as Poor. Since the dataset does not provide actual review text, keyword and review-length analysis could not be performed.

Task 2 — Votes Analysis

Objectives

Identify the restaurants with the highest and lowest number of votes.

Analyze whether votes are related to restaurant ratings.

Calculate the correlation between votes and aggregate rating.

Results

Highest-voted restaurant: Toit

Votes: 10,934

Rating: 4.8

Lowest-voted restaurant: Cantinho da Gula

Votes: 0

Rating: 0.0

Correlation between Votes and Aggregate Rating: 0.3137

Conclusion

The correlation coefficient of 0.3137 indicates a weak positive relationship between the number of votes and restaurant ratings. Restaurants with higher ratings tend to receive somewhat more votes, but the relationship is not strong. Therefore, the number of votes alone is not a strong predictor of a restaurant's rating.

Task 3 — Price Range vs. Online Delivery and Table Booking

Objectives

Analyze the relationship between price range and online delivery availability.

Analyze the relationship between price range and table booking availability.

Determine whether higher-priced restaurants are more likely to provide these services.

Results

Price Range

Online Delivery

Table Booking

1

15.77%

0.02%

2

41.31%

7.68%

3

29.19%

45.74%

4

9.04%

46.76%

Lowest price range: 1

Highest price range: 4

Conclusion

Table booking availability increases strongly with price range, rising from only 0.02% for Price Range 1 to 46.76% for Price Range 4. Online delivery does not show the same increasing pattern. It is highest for Price Range 2 at 41.31% and lowest for Price Range 4 at 9.04%.

Therefore, higher-priced restaurants are considerably more likely to offer table booking, but higher prices do not consistently indicate greater availability of online delivery.

Skills Demonstrated

Exploratory Data Analysis (EDA)

Data Cleaning and Preparation

Statistical Analysis

Correlation Analysis

Data Aggregation and Grouping

Categorical Data Analysis

Restaurant Rating Analysis

Cuisine Analysis

Restaurant Chain Analysis

Geographic Data Visualization

Interactive Mapping with Folium

Data Visualization

Python Programming

Pandas and NumPy

Matplotlib and Seaborn

Jupyter Notebook

How to Run

1. Create the virtual environment

python -m venv .venv

2. Activate the virtual environment on Windows

.\.venv\Scripts\Activate.ps1

3. Install required libraries

python -m pip install pandas numpy matplotlib seaborn folium jupyter ipykernel

4. Start Jupyter Notebook

python -m jupyter notebook

Alternatively, open the notebooks directly in VS Code and select:

.venv (Python 3.14)

5. Run the notebooks

Run the notebooks in this order:

Level_1/Level_1_Analysis.ipynb
Level_2/Level_2_Analysis.ipynb
Level_3/Level_3_Analysis.ipynb

The dataset should be located at:

Dataset/Dataset.csv

Overall Conclusion

The Cognifyz Data Analysis project provided practical experience in analyzing a real-world restaurant dataset. Across three levels, the project covered restaurant ratings, cuisines, cities, pricing, online delivery, geographic distribution, restaurant chains, rating categories, votes, and service availability.

The analysis demonstrates practical skills in data preprocessing, exploratory data analysis, statistical analysis, correlation analysis, visualization, geographic mapping, and communicating data-driven insights.