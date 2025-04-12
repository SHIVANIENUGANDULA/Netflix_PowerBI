# 🍿 Netflix Data Analysis Dashboard - Power BI Project
![Netflix Logo](logo.png)
This Power BI project analyzes viewing and content trends on the Netflix platform using a structured dataset. The interactive dashboard showcases KPIs, content classification, and insights across various genres, countries, and release years.

---

## 🎯 Project Objectives

- Visualize the distribution of content across genres, types, and countries  
- Analyze content release trends over time  
- Identify the most frequent actors and directors  
- Track content availability across years and platforms  
- Provide dynamic filtering by year, genre, country, and rating  

---

## 🧾 Dataset Description

The dataset includes fields such as:

- Title, Type (Movie/TV Show)  
- Country of origin  
- Date Added to Netflix  
- Release Year  
- Rating (e.g., TV-MA, PG-13)  
- Duration (mins or seasons)  
- Genre and Cast information  

📦 **Source**: [Netflix TV Shows and Movie List – Kaggle](https://www.kaggle.com/datasets/snehaanbhawal/netflix-tv-shows-and-movie-list)

> *This dataset is publicly available and widely used for Netflix content analysis.*

---

## 📊 Dashboard Features

- 📅 Content by Year and Type  
- 🌍 Country-wise distribution of titles  
- 🎭 Top 10 Genres and Ratings  
- 🧑‍🤝‍🧑 Most Frequent Actors and Directors  
- 🧰 Interactive filtering and drill-down  

---

## 🧠 DAX Formulas (Examples)

```dax
Total Titles = COUNTROWS(Netflix)

Movies Count = CALCULATE(COUNTROWS(Netflix), Netflix[Type] = "Movie")

TV Shows Count = CALCULATE(COUNTROWS(Netflix), Netflix[Type] = "TV Show")

Top Country = 
    CALCULATE(
        COUNT(Netflix[Title]), 
        ALLEXCEPT(Netflix, Netflix[Country])
    )
```
> *You can find more DAX formulas in .pbix file


📘 References:
- [DAX Guide](https://dax.guide/)
- [Microsoft Learn - Power BI](https://learn.microsoft.com/en-us/power-bi/)

---

## 🛠 Tools Used

- Power BI Desktop  
- Power Query (for data cleaning)  
- DAX (for metrics and aggregations)  
- Data modeling and visualization  

---

## 📁 Repository Structure

```
📁 Netflix-PowerBI-Project
│
├── README.md
├── NETFLIX.pbix
├── 📁 Netflix_Listings.xlsx
├── 📁 Images (Background & logos)
│
```

---

## 📌 Author

**Shivani Enugandula**  
🔗 [LinkedIn](https://www.linkedin.com/in/shivani-enugandula/)

---

This project is ideal for showcasing Power BI development skills, DAX proficiency, and storytelling with data using a popular real-world use case.
