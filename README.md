# Netflix Exploratory Data Analysis  
**Phases 1 & 2: Data Cleaning, Preprocessing & Exploratory Data Analysis**

This project explores the Netflix catalog to uncover trends in content types, ratings, genres, and countries of origin.  
It is part of my personal data science portfolio.

## 🎯 Objectives
- Perform data cleaning and preprocessing  
- Conduct exploratory data analysis (EDA)  
- Visualize trends in Netflix content by year, rating, and category  
- Develop data storytelling skills and generate actionable insights  

## 🧰 Tools Used
- Python (Pandas, NumPy, Matplotlib, Seaborn, Plotly)  
- Jupyter Notebook  
- Visual Studio Code (VS Code)  

## 📁 Project Structure
- `netflix_titles.csv`  
- `netflix_cleaned_v2.csv`  
- `Netflix_EDA.ipynb`  
- `/images/`  
- `README.md`  

## 🗂️ Dataset
The dataset is sourced from Kaggle: [Netflix Dataset](https://www.kaggle.com/datasets/rohitgrewal/netflix-data/data?select=Netflix+Dataset.csv)

## 🚀 Progress Tracker
- Phase 1: Data cleaning and preprocessing — Completed  
- Phase 2: Exploratory data analysis and visualization — Completed  
- Phase 3: Statistical & predictive analysis — In progress  

## 📊 Key Insights & Findings from Phase 2
- The majority of Netflix content consists of movies, with TV shows making up a smaller but significant portion.  
- Content ratings show a strong preference for mature audiences, with many titles rated TV-MA or equivalent.  
- Popular genres include Drama, Comedy, and Thriller, with a growing trend in documentaries in recent years.  
- The United States, India, and the United Kingdom are the top countries producing Netflix content, reflecting both regional preferences and production investments.  
- Release year analysis reveals an increasing volume of content added annually, especially after 2015, indicating Netflix’s expansion strategy.  
- Visualizations highlight distinct patterns in content type distribution over time and by rating category, enabling targeted content recommendations.  

## 🤖 Phase 3: Statistical & Predictive Analysis

In this phase, we transitioned from exploratory data analysis to **predictive modeling** using machine learning techniques.  
The goal was to determine whether a title is a **Movie or a TV Show** based on selected attributes such as rating, country, duration, and release year.

### 🔍 Approach
- Conducted **statistical exploration** to identify meaningful numeric and categorical relationships.  
- Applied **Random Forest Classification** to predict the content type (Movie vs TV Show).  
- Evaluated model accuracy and feature importance to interpret predictive relationships.

### 📊 Key Results
- The **Random Forest model achieved 100% accuracy**, demonstrating a clear distinction between Movies and TV Shows.  
- **Duration** emerged as the dominant predictive feature, accounting for over **90% of feature importance**.  
  - *Interpretation:* Movies are represented in minutes (e.g., “93 min”) while TV Shows are defined in seasons (e.g., “4 Seasons”).  
- Other features such as **Rating** and **Country** contributed minor predictive value, while **Year** showed negligible impact.  
- The results underscore the importance of **feature representation** — seemingly simple attributes like “Duration” can carry strong classification power.

### 🚀 Next Steps (Completed)

Following the initial Random Forest classification, further steps were taken to validate and expand the analysis:

#### Phase 3 – Part 2: Statistical Validation & Model Comparison
To ensure the Random Forest’s accuracy was not misleading, statistical validation and model comparison were performed.

**Highlights:**
- The **average movie duration** was ~99 minutes, while TV shows averaged ~1.7 (season units).  
- A **t-test** confirmed a statistically significant difference (p-value = 0.0), validating that `Duration` alone strongly separates categories.  
- Alternative models — **Logistic Regression** and **XGBoost** — were tested, achieving nearly identical accuracies (~99.8%), confirming the simplicity of this classification problem.  

**Key Lesson:**  
This phase emphasized how data structure (e.g., how durations are encoded) can heavily influence model outcomes.  
Understanding feature representation is crucial before drawing conclusions from predictive performance.

---

### 🔮 Upcoming Work – Phase 3 Part 3 (Regression Analysis)
Next, the project transitions from classification to regression:
- Develop **Linear Regression** and **Random Forest Regressor** models.  
- Predict movie durations using attributes such as rating, release year, and country.  
- Evaluate using **MAE**, **RMSE**, and **R²**, visualizing predictions vs actual values.  

This will provide hands-on practice with regression modeling and demonstrate predictive insight beyond categorical classification.

---

### Phase 3 – Part 3: Regression Analysis (Completed)

This final segment of Phase 3 applied regression techniques to predict **movie durations** based on their rating, country, and release year.

#### Model Performance
| Model | MAE | RMSE | R² |
|:------|:----:|:----:|:---:|
| Linear Regression | 19.25 | 25.91 | 0.150 |
| Random Forest Regressor | **16.05** | **22.31** | **0.370** |

#### Key Insights
- **Random Forest** outperformed Linear Regression, capturing non-linear effects in the data.  
- Despite improvement, both models indicate that duration is influenced by more than just rating or release year.  
- The **Actual vs Predicted** visualization shows clustering around standard movie lengths (80–120 minutes), confirming realistic model behavior.  
- These findings emphasize the balance between **model complexity** and **data completeness**.

📈 *Conclusion:*  
Regression analysis completes the Netflix EDA and Predictive Modeling pipeline — covering cleaning, visualization, classification, and regression in one cohesive, end-to-end project.

---

## 🖼️ Visual Gallery
- Content Type Distribution Over Years  
- Ratings Breakdown by Content Type  
- Genre Popularity Trends  
- Country of Origin Analysis  
- Yearly Content Release Volume  
- Interactive Dashboard of Netflix Titles by Various Attributes  

---

## 🎬 Final Project Summary

This project represents a complete data science workflow applied to the **Netflix Movies and TV Shows Dataset**.  
It spans from **data cleaning** and **exploratory analysis** to **statistical validation** and **predictive modeling**, showcasing both technical ability and interpretive clarity.

Key takeaways include:
- A clear structural difference between movies and TV shows, primarily driven by duration.  
- Netflix’s content surge post-2015, reflecting global platform expansion.  
- Successful implementation of classification and regression models, with **Random Forest** emerging as the most adaptable and accurate approach.  
- Demonstrated proficiency in **EDA, visualization, and model evaluation** — essential skills for data analysis and machine learning roles.

This project serves as the foundation for the upcoming portfolio series, each designed to highlight a different facet of applied data science using real-world datasets.