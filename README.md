# Film-Audience-Preference-Association-Engine
Applies association rule mining to audience movie preference data to identify viewing patterns, group consumer clusters, and optimize targeted film distribution strategies.


# 🎬 Film Distribution: Audience Preference Analysis & Association Mining

## 1. Business Problem

### 1.1. What is the business objective?
* **Audience Targeting:** Help a film distribution company target audiences more effectively based on their movie likes, dislikes, and viewing preferences.
* **Association Rule Generation:** Uncover viewing patterns and hidden relationships between different movie titles or genres to optimize film clustering, distribution strategies, and content recommendation campaigns.

### 1.2. Are there any constraints?
* **Sparse Preferences:** Managing binary or categorical preference data where viewers may only express likes for a small subset of available films.
* **Metric Thresholds:** Carefully tuning support, confidence, and lift parameters to avoid overwhelming marketing teams with redundant rules while capturing niche audience segments.

---

## 2. Data Dictionary (`my_movies.csv`)

| Feature Name | Data Type | Description |
| :--- | :--- | :--- |
| **User_ID / Customer_ID** | Integer / String | Unique identifier for each viewer or survey respondent. |
| **Movie Titles / Genres** | Categorical / Binary | Indicators representing whether a user likes, dislikes, or has watched specific films. |

---

## 3. Data Pre-processing

### 3.1. Data Cleaning & Feature Engineering
* **Data Transformation:** Processed raw viewer feedback and movie lists into a structured boolean or one-hot encoded matrix suitable for association rule mining.
* **Data Sanitization:** Handled missing responses and standardized movie title formatting across records.

---

## 4. Model Building

### 4.1. Application of Apriori Algorithm
* Implemented the Apriori algorithm using Python (e.g., `mlxtend`) to extract frequent movie itemsets meeting the minimum support threshold.
* Filtered and evaluated rules using **Confidence** and **Lift** to determine strong associations between movie preferences.

### 4.2. Frequent Itemsets & Rule Visualization
* Generated frequent itemset combinations and created scatter plots and network graphs to map out audience preference affinities clearly.

### 4.3. Work on Codes
* The complete source code implementation is stored in the `My_Movies.py` file.

---

## 5. Deployment

### 5.1. Deploy Solutions
* The association rules can be integrated into a recommendation engine dashboard for marketing teams or utilized for targeted digital advertising campaigns on streaming and distribution platforms.

---

## 6. Business Impact & Benefits
* **Precision Marketing:** Enables the distribution team to run targeted campaigns recommending film bundles or sequels to audiences based on past preferences.
* **Improved Acquisition:** Increases viewer engagement and ticket or subscription sales by aligning content promotion with proven viewer taste clusters.
