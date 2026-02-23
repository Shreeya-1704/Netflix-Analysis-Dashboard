# Netflix-Analysis-Dashboard
This project analyzes Netflix movies and TV shows data to uncover content trends, genre popularity, and country-wise distribution.
Using Power BI for data transformation and visualization, the dashboard highlights content growth, ratings distribution, and genre performance to support data-driven insights.

Problem Statement
Streaming platforms need to understand content trends, audience preferences, and distribution to improve content strategy and user engagement.
This project identifies total titles, popular genres, ratings distribution, and release trends to help analyze Netflix’s content library.

Tools & Skills
Power BI (data cleaning, transformation, and interactive dashboards)

Workflow
Imported Netflix dataset into Power BI.
Transformed data (handled missing values, created calculated columns such as Duration in mins and First Category).
Built interactive dashboards showing KPIs, release trends, genre distribution, and country-wise analysis.
Summarized insights to understand content growth and distribution.

Potential Extensions with SQL

Although this project was built entirely in Power BI, SQL could be used in a real-world scenario to query data directly from the database:

-- Total number of titles
SELECT COUNT(show_id) AS TotalTitles
FROM netflix_titles;

-- Titles released per year
SELECT release_year, COUNT(show_id) AS TotalTitles
FROM netflix_titles
GROUP BY release_year;

-- Top genres by total titles
SELECT listed_in, COUNT(show_id) AS TotalTitles
FROM netflix_titles
GROUP BY listed_in
ORDER BY TotalTitles DESC;

-- Rating distribution
SELECT rating, COUNT(show_id) AS TotalTitles
FROM netflix_titles
GROUP BY rating;

This dashboard helps understand Netflix content distribution, growth trends, and audience targeting. It demonstrates skills in Power BI, data analysis, and dashboard design, making it suitable for data analyst and business intelligence roles.
