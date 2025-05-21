# Google Play Store Apps Analysis and Visualization

This project explores trends, patterns, and distributions in the Google Play Store using data cleaning, feature transformation, and visualization techniques. It aims to understand what makes apps successful by examining factors such as installs, ratings, reviews, categories, and genres.

---

## Project Objectives

- Clean and preprocess raw Google Play Store data.
- Perform exploratory data analysis (EDA) to uncover patterns across installs, ratings, and app categories.
- Visualize relationships between features using plots and heatmaps.
- Derive insights into top-performing genres, app pricing, and popularity metrics.

---

## Tools and Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- SciPy (for statistical analysis)
- Jupyter Notebook or Google Colab

---

## Dataset

- Source: Google Play Store Dataset (CSV format)
- Features include:
  - App, Category, Rating, Reviews, Size, Installs, Type, Price, Content Rating, Genres, Last Updated, Current Version, Android Version

---

## Project Workflow

### 1. Data Cleaning

- Removed duplicate rows and fixed data formatting issues.
- Dropped or filled missing values:
  - Missing `Rating` values filled using install category-based averages.
  - Converted `Reviews` to integers and cleaned `Price` and `Size`.
- Created new feature `Size_MB` from the original `Size` column.
- Dropped non-essential rows with inconsistent or missing critical data.

### 2. Feature Engineering

- Created a new `Installs_category` feature by binning install counts into labeled ranges.
- Extracted and cleaned genre data from the `listed_in` column.

### 3. Exploratory Data Analysis (EDA)

- Visualized:
  - App distribution by type (Free vs. Paid)
  - Most common genres and categories
  - Relationship between installs and ratings
  - Ratings by install volume categories
  - Review volume and content ratings
- Plotted:
  - Correlation matrix among numerical variables
  - Boxplots and countplots across categories
  - Word cloud from app titles

---

## Key Findings

- Most apps on the Play Store are free and belong to the FAMILY or GAME category.
- Apps in the EDUCATION, EVENTS, and BOOKS_AND_REFERENCE categories had the highest average ratings.
- High install counts correlate moderately with high review counts.
- Paid apps are fewer but exist across various categories.
- Most apps are rated between 4.0 and 4.5, indicating generally positive user experiences.

---

## Future Enhancements

- Add sentiment analysis using app descriptions or user reviews.
- Build classification or regression models to predict app success.
- Develop interactive dashboards using Plotly or Tableau.
- Incorporate time-series data to analyze app trends over time.
- Use clustering to group apps based on features and user behavior.

---

## Author

**TARUN C**  
Data Analyst intern
UNIFIED MENTOR
