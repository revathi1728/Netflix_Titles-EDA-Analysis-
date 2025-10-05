# 🍿 Netflix Movies & TV Shows — Exploratory Data Analysis (EDA)

This project presents a **comprehensive Exploratory Data Analysis (EDA)** of the Netflix Titles dataset.  
It explores the types, genres, release trends, and durations of movies and TV shows available on Netflix.

---

## 📘 Project Overview

The goal of this analysis is to uncover patterns and insights from the Netflix content catalog, such as:
- Which countries and genres dominate Netflix content?
- How has content production evolved over the years?
- What’s the difference between movies and TV shows in terms of duration?
- How can we visualize Netflix’s global content diversity?

This notebook demonstrates essential EDA steps: **data cleaning, transformation, visualization, and interpretation** — perfect for beginners in Data Science.

---

## 🧩 Dataset Information

**Dataset name:** `netflix_titles.csv`  
**Source:** [Netflix Titles Dataset on Kaggle](https://www.kaggle.com/shivamb/netflix-shows)  
**Rows:** ~8,800  
**Columns include:**
- `show_id` – Unique ID for each title  
- `type` – Movie or TV Show  
- `title` – Title of the content  
- `director` – Director name(s)  
- `cast` – Main actors  
- `country` – Country of origin  
- `date_added` – Date added to Netflix  
- `release_year` – Year of release  
- `rating` – Content rating (e.g., TV-MA, PG-13)  
- `duration` – Duration (minutes for movies or seasons for TV shows)  
- `listed_in` – Genre/category  
- `description` – Short summary

---

## 🧠 EDA Workflow

### 1️⃣ Data Setup & Loading
- Imported Python libraries: `Pandas`, `NumPy`, `Matplotlib`, `Seaborn`
- Loaded dataset and viewed structure, shape, and data types.

### 2️⃣ Data Cleaning
- Removed **missing values** and **duplicates**.
- Checked column data types and consistency.
- Added a new column `duration_mins` for unified duration representation.

### 3️⃣ Feature Engineering
Converted “duration” text into numeric form:
- Movies → Minutes  
- TV Shows → Estimated total minutes (`seasons × 450` minutes)

### 4️⃣ Univariate Analysis
- Distribution of content type (Movies vs TV Shows)
- Number of titles released by year
- Top 10 producing countries
- Most frequent genres (`listed_in`)

### 5️⃣ Bivariate Analysis
- Relationship between **release decade** and **type**
- Boxplots comparing movie and TV show durations

---

## 📊 Visualizations

The notebook includes:
- 📈 **Line Plot:** Content growth by release year  
- 📊 **Bar Charts:** Top countries, top genres  
- 🧮 **Count Plot:** Movies vs TV Shows by decade  
- 📦 **Boxplots:** Duration comparison  
- 🌸 **Seaborn Themes:** Used for clarity and modern visualization  

---

## 🏁 Key Insights & Conclusion

✅ **Movies dominate** the Netflix catalog, but **TV Shows** have steadily grown over recent decades.  
✅ Most content comes from **the U.S., India, and the U.K.**, showing strong international presence.  
✅ Common genres include **Drama**, **Comedy**, and **Documentary** — reflecting global storytelling trends.  
✅ Movie durations mostly range **between 90–120 minutes**, while TV shows average **1–3 seasons**.  
✅ The dataset demonstrates Netflix’s shift toward regional and series-based content diversity.

---

## 🚀 Future Enhancements
- Add **rating-based visualizations** (e.g., PG-13 vs TV-MA).  
- Perform **text analysis** on descriptions to find trending keywords.  
- Build **interactive dashboards** using Plotly or Power BI.  
- Predict popular genres using basic machine learning.

---

## 🛠️ Tech Stack
- **Python**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- *(Optional)* Plotly for interactive charts

---

## 📂 Repository Structure

