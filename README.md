# 🍽️ Cognifyz Data Analysis Internship

## 📌 Overview

This project contains my **Data Analysis Internship work at Cognifyz Technologies**.

The project analyzes a restaurant dataset containing **9,551 records and 21 attributes** using Python and popular data analysis and visualization libraries.

The analysis is divided into **three levels**, covering exploratory data analysis, restaurant ratings, cuisine combinations, geographic analysis, restaurant chains, votes, reviews, pricing, online delivery, and table booking.

---

## 🛠️ Technologies Used

- Python 3.14
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Folium

---

# 📁 Project Structure

```text
Cognifyz-Data-Analysis/
│
├── Dataset/
│   └── Dataset.csv
│
├── Level_1/
│   ├── Level_1_Analysis.ipynb
│   ├── city_analysis.png
│   ├── online_delivery.png
│   ├── price_distribution.png
│   ├── rating_distribution.png
│   └── top_cuisines.png
│
├── Level_2/
│   ├── Level_2_Analysis.ipynb
│   ├── chain_analysis.png
│   ├── cuisine_combination_ratings.png
│   ├── cuisine_combinations.png
│   ├── rating_distribution.png
│   ├── restaurant_chains.png
│   └── restaurant_map.html
│
├── Level_3/
│   ├── Level_3_Analysis.ipynb
│   │
│   ├── Task_1_Restaurant_Reviews/
│   │   ├── rating_text_distribution.png
│   │   └── review_analysis_note.txt
│   │
│   ├── Task_2_Votes_Analysis/
│   │   ├── top_voted_restaurants.png
│   │   └── votes_vs_rating.png
│   │
│   └── Task_3_Price_Range_Services/
│       ├── online_delivery_by_price.png
│       └── table_booking_by_price.png
│
├── .gitignore
└── README.md
```

---

# 📊 Level 1 — Exploratory Data Analysis

## Task 1 — Top Cuisines

### 🎯 Objectives

- Identify the most common cuisines.
- Calculate their prevalence in the dataset.
- Visualize cuisine popularity.

### 📌 Conclusion

The analysis identified **North Indian, Chinese Cuisine, and Fast Food** as some of the most commonly occurring cuisines. North Indian cuisine had the highest prevalence among the analyzed cuisines, showing its strong presence in the restaurant dataset.

---

## Task 2 — City Analysis

### 🎯 Objectives

- Identify the city with the highest number of restaurants.
- Calculate the average rating of restaurants in that city.
- Visualize restaurant distribution by city.

### 📌 Results

| Metric | Result |
|---|---|
| City with highest number of restaurants | New Delhi |
| Number of restaurants | 5,473 |
| Average rating | 2.44 |

### 📌 Conclusion

**New Delhi** has the highest number of restaurants in the dataset, with **5,473 restaurants**. However, its average rating is **2.44**, showing that having a large number of restaurants does not necessarily mean having higher average ratings.

---

## Task 3 — Price Range Distribution

### 🎯 Objectives

- Determine the most common price range.
- Calculate the number of restaurants in each price category.
- Calculate the percentage distribution.
- Visualize the price range distribution.

### 📌 Results

| Metric | Result |
|---|---|
| Most common price range | 1 |
| Number of restaurants | 4,444 |
| Percentage | 46.53% |

### 📌 Conclusion

**Price Range 1** is the most common category, containing **4,444 restaurants** and representing **46.53%** of the dataset. This indicates that a large proportion of restaurants belong to the lower price category.

---

## Task 4 — Online Delivery

### 🎯 Objectives

- Analyze the availability of online delivery.
- Compare restaurants with and without online delivery.
- Compare average ratings based on online delivery availability.

### 📌 Results

| Online Delivery | Number of Restaurants |
|---|---:|
| No | 7,100 |
| Yes | 2,451 |

| Online Delivery | Average Rating |
|---|---:|
| No | 2.47 |
| Yes | 3.25 |

### 📌 Conclusion

Most restaurants in the dataset **do not provide online delivery**, with 7,100 restaurants compared to 2,451 that do.

Restaurants offering online delivery have a higher average rating of **3.25**, compared with **2.47** for restaurants without online delivery.

---

## Task 5 — Restaurant Ratings

### 🎯 Objectives

- Analyze the distribution of restaurant ratings.
- Identify the most common rating range.
- Calculate the average number of votes received by restaurants.

### 📌 Results

| Rating Range | Restaurant Count | Percentage |
|---|---:|---:|
| 0–1 | 2,148 | 22.49% |
| 1–2 | 10 | 0.10% |
| 2–3 | 1,891 | 19.80% |
| 3–4 | 4,388 | 45.94% |
| 4–5 | 1,114 | 11.66% |

**Average number of votes per restaurant:** `156.91`

### 📌 Conclusion

The **3–4 rating range** is the most common category, containing **4,388 restaurants** and representing **45.94%** of the dataset. The average restaurant receives approximately **156.91 votes**.

---

# 📈 Level 2 — Advanced Analysis

## Task 1 — Restaurant Ratings

### 🎯 Objectives

- Analyze the distribution of aggregate ratings.
- Determine the most common rating range.
- Calculate the average number of votes received by restaurants.

### 📌 Results

| Rating Range | Restaurant Count | Percentage |
|---|---:|---:|
| 0–1 | 2,148 | 22.49% |
| 1–2 | 10 | 0.10% |
| 2–3 | 1,891 | 19.80% |
| 3–4 | 4,388 | 45.94% |
| 4–5 | 1,114 | 11.66% |

- **Most common rating range:** 3–4
- **Restaurants:** 4,388
- **Percentage:** 45.94%
- **Average number of votes:** 156.91

### 📌 Conclusion

The **3–4 rating range** is the most common rating category, accounting for **45.94%** of restaurants. This indicates that most rated restaurants fall within the moderate-to-good rating range.

---

## Task 2 — Cuisine Combinations

### 🎯 Objectives

- Identify common cuisine combinations.
- Analyze the ratings of cuisine combinations.
- Identify the highest-rated cuisine combination.

### 📌 Results

| Metric | Result |
|---|---|
| Highest-rated cuisine combination | Modern Indian |
| Average rating | 4.35 |
| Number of restaurants | 11 |

### 📌 Conclusion

The analysis shows that cuisine popularity and customer ratings do not necessarily have a direct relationship.

The **Modern Indian** cuisine combination achieved the highest average rating of **4.35**, based on **11 restaurants**.

---

## Task 3 — Geographic Analysis

### 🎯 Objectives

- Analyze the geographic distribution of restaurants.
- Use latitude and longitude to visualize restaurant locations.
- Identify areas with high restaurant concentration.
- Create an interactive restaurant map.

### 📌 Results

An interactive geographic visualization was created using **Folium**.

The generated map is saved as:

```text
Level_2/restaurant_map.html
```

### 📌 Conclusion

The geographic analysis shows that restaurants are concentrated in major urban areas. The interactive map provides a visual representation of restaurant locations and helps identify areas with higher restaurant density.

---

## Task 4 — Restaurant Chains

### 🎯 Objectives

- Identify the most popular restaurant chains.
- Determine the number of restaurants belonging to major chains.
- Compare popularity with average ratings.
- Identify the highest-rated restaurant chain.

### 📌 Results

| Metric | Result |
|---|---|
| Most popular restaurant chain | Cafe Coffee Day |
| Number of restaurants | 83 |
| Highest-rated restaurant chain | Barbeque Nation |
| Average rating | 4.35 |

### 📌 Conclusion

**Cafe Coffee Day** has the largest presence in the dataset with **83 restaurants**, while **Barbeque Nation** achieved the highest average rating of **4.35**.

This demonstrates that restaurant popularity and customer ratings do not necessarily go hand in hand.

---

# 🚀 Level 3 — Advanced Analysis

## Task 1 — Restaurant Reviews

### 🎯 Objectives

- Analyze text reviews to identify common positive and negative keywords.
- Calculate the average length of reviews.
- Explore the relationship between review length and rating.

### ⚠️ Dataset Limitation

The provided dataset does not contain a dedicated **text-review column**.

Therefore, actual positive/negative keyword extraction, review-length calculation, and review-length versus rating analysis could not be reliably performed.

Instead, the available **`Rating text`** column was analyzed.

### 📌 Results

| Rating Text | Percentage |
|---|---:|
| Average | 39.13% |
| Not rated | 22.49% |
| Good | 21.99% |
| Very Good | 11.30% |
| Excellent | 3.15% |
| Poor | 1.95% |

### 📌 Conclusion

**Average** is the most common rating category at **39.13%**, followed by **Not rated** at **22.49%** and **Good** at **21.99%**.

Only **3.15%** of restaurants are categorized as Excellent, while **1.95%** are categorized as Poor.

Since the dataset does not contain actual review text, keyword and review-length analysis could not be performed.

---

## Task 2 — Votes Analysis

### 🎯 Objectives

- Identify restaurants with the highest number of votes.
- Identify restaurants with the lowest number of votes.
- Analyze the relationship between votes and restaurant ratings.
- Calculate the correlation between votes and aggregate rating.

### 📌 Results

| Metric | Result |
|---|---|
| Highest-voted restaurant | Toit |
| Highest votes | 10,934 |
| Rating of highest-voted restaurant | 4.8 |
| Lowest-voted restaurant | Cantinho da Gula |
| Lowest votes | 0 |
| Rating of lowest-voted restaurant | 0.0 |
| Correlation between votes and rating | 0.3137 |

### 📌 Conclusion

The correlation coefficient of **0.3137** indicates a **weak positive relationship** between the number of votes and restaurant ratings.

Restaurants with higher ratings tend to receive somewhat more votes, but the relationship is not strong. Therefore, the number of votes alone is not a strong predictor of a restaurant's rating.

---

## Task 3 — Price Range vs. Online Delivery and Table Booking

### 🎯 Objectives

- Analyze the relationship between price range and online delivery.
- Analyze the relationship between price range and table booking.
- Determine whether higher-priced restaurants are more likely to offer these services.

### 📌 Results

| Price Range | Online Delivery | Table Booking |
|---|---:|---:|
| 1 | 15.77% | 0.02% |
| 2 | 41.31% | 7.68% |
| 3 | 29.19% | 45.74% |
| 4 | 9.04% | 46.76% |

### 📌 Conclusion

Table booking availability increases strongly with price range, rising from **0.02% in Price Range 1** to **46.76% in Price Range 4**.

Online delivery does not follow the same pattern. It is highest in **Price Range 2 at 41.31%** and lowest in **Price Range 4 at 9.04%**.

Therefore, higher-priced restaurants are considerably more likely to offer **table booking**, but higher prices do not consistently indicate greater availability of **online delivery**.

---

# 💡 Key Insights

- **New Delhi** has the highest number of restaurants in the dataset.
- **Price Range 1** is the most common price category.
- Restaurants offering **online delivery have a higher average rating** than those without it.
- The **3–4 rating range** contains the largest number of restaurants.
- **Modern Indian** is the highest-rated cuisine combination in the analysis.
- **Cafe Coffee Day** is the most widely represented restaurant chain.
- **Barbeque Nation** has the highest average rating among the analyzed chains.
- There is a **weak positive correlation** between votes and ratings.
- Higher-priced restaurants are much more likely to offer **table booking**.
- Online delivery availability does not consistently increase with price.

---

# 🧠 Skills Demonstrated

- Exploratory Data Analysis (EDA)
- Data Cleaning and Preparation
- Statistical Analysis
- Correlation Analysis
- Data Aggregation and Grouping
- Categorical Data Analysis
- Restaurant Rating Analysis
- Cuisine Analysis
- Restaurant Chain Analysis
- Geographic Data Visualization
- Interactive Mapping
- Data Visualization
- Python Programming
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Folium
- Jupyter Notebook

---

# ⚙️ How to Run the Project

## 1. Clone the Repository

```bash
git clone https://github.com/Nilakshi15/Cognifyz-Data-Analysis.git
```

## 2. Navigate to the Project

```bash
cd Cognifyz-Data-Analysis
```

## 3. Create a Virtual Environment

```powershell
python -m venv .venv
```

## 4. Activate the Virtual Environment

For Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

## 5. Install Required Libraries

```powershell
python -m pip install pandas numpy matplotlib seaborn folium jupyter ipykernel
```

## 6. Start Jupyter Notebook

```powershell
python -m jupyter notebook
```

Alternatively, the notebooks can be opened directly in VS Code using the **Python 3.14 virtual environment** as the kernel.

---

# ▶️ Notebook Execution Order

Run the notebooks in the following order:

```text
1. Level_1/Level_1_Analysis.ipynb
2. Level_2/Level_2_Analysis.ipynb
3. Level_3/Level_3_Analysis.ipynb
```

The dataset should be available at:

```text
Dataset/Dataset.csv
```

---

# 📌 Overall Conclusion

The Cognifyz Data Analysis project provided practical experience in working with a real-world restaurant dataset.

Across three levels, the project covered:

- Restaurant distribution
- Cities
- Cuisines
- Price ranges
- Ratings
- Online delivery
- Geographic distribution
- Restaurant chains
- Votes
- Review categories
- Table booking

The project demonstrates practical skills in **data preprocessing, exploratory data analysis, statistical analysis, correlation analysis, data visualization, geographic visualization, and communicating data-driven insights**.

---

## 👩‍💻 Author

**Nilakshi Patil**

Computer Engineering Student  
PCCOE