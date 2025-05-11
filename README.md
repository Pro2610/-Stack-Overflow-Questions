# 📊 Stack Overflow Questions Analysis

This project explores patterns and trends in technical questions asked on Stack Overflow using Google's BigQuery and the public dataset `bigquery-public-data.stackoverflow.posts_questions`.

## 🚀 Project Overview

The goal of this project is to analyze the evolution of programming topics, question popularity, and community engagement over time.

Main tools used:
- 🧮 BigQuery (SQL)
- 📊 Tableau / Google Sheets (for data visualization)
- 📝 GitHub (for documentation and project sharing)

## 📚 Dataset

- **Source:** [Google BigQuery Public Dataset](https://console.cloud.google.com/marketplace/product/bigquery-public/stackoverflow)
- **Table:** `bigquery-public-data.stackoverflow.posts_questions`
- Fields include: question title, creation date, tags, score, view count, number of answers, and more.

## 🔍 Key Questions & Analyses

- 📅 How many questions are asked per year?
- 🏷️ What are the most popular programming tags?
- 💡 Which tags have the highest average scores?
- 🔥 Which technologies are growing the fastest?
- 🤔 How many questions receive no answers?

## 🛠️ Sample SQL Queries

```sql
-- Questions per year
SELECT EXTRACT(YEAR FROM creation_date) AS year, COUNT(*) AS total
FROM `bigquery-public-data.stackoverflow.posts_questions`
GROUP BY year
ORDER BY year;

📈 Visualizations
Visualizations were built in Tableau (or Google Sheets), including:

Line chart: Questions per year

Bar chart: Top 10 tags

Table: Questions with the highest view count

Heatmap: Tag trends over time



🧑‍💻 Author
Yana Prozhuhan
https://www.linkedin.com/in/yana-prozhuhan/
