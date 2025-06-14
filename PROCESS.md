# Process Documentation

## 1. Data Extraction (E)

The dataset was sourced from Kaggle’s [Netflix Movies and TV Shows dataset](https://www.kaggle.com/shivamb/netflix-shows). It was provided as a CSV file containing information such as show titles, release years, genres, countries, and ratings. The data was loaded into the project using the pandas library.

**Challenges:**  
- The dataset contained some missing values in key columns such as `cast` and `country`.  
- Some entries had inconsistent formatting in date and categorical fields.

**Solutions:**  
- Utilized `pandas` functions like `.isnull()` to identify missing values.  
- Applied appropriate handling such as filling missing data with placeholders or dropping rows where necessary.  
- Standardized date formats using `pd.to_datetime()` to ensure consistency.

## 2. Data Transformation (T)

Data cleaning involved several steps:

- Removed duplicate entries to avoid skewing analysis.  
- Filled missing values in `rating` and `cast` columns with “Not Specified” to maintain dataset integrity.  
- Converted date fields to datetime objects for easier filtering and visualization.  
- Created new features such as `release_decade` by extracting the decade from the release year to analyze trends over time.  
- Filtered data to focus on specific content types like movies or TV shows as required.

**Challenges:**  
- Handling multiple values in fields like `genre` and `cast` which were stored as comma-separated strings.  
- Inconsistent country names and missing data complicated geographic analysis.

**Solutions:**  
- Split multi-value fields into lists for better filtering and grouping.  
- Standardized country names using mapping dictionaries to unify similar entries.

## 3. Data Loading (L)

After cleaning and transformation, the processed data was directly used within the Jupyter Notebook for analysis and visualization. No external database was used; however, the cleaned dataset was optionally saved as a new CSV file for future reuse.

**Challenges:**  
- Large dataset size occasionally slowed down processing during visualization.

**Solutions:**  
- Applied filters and subsetted the data to smaller chunks when visualizing to improve performance.

## 4. Visualization Process

The analysis utilized the following Python libraries:

- **Matplotlib** and **Seaborn** for static visualizations such as bar charts, histograms, and pie charts.  
- **Plotly Express** for interactive charts to explore trends dynamically.

Key visualizations included:

- Distribution of content types (Movies vs TV Shows)  
- Number of shows released per year and decade  
- Genre popularity breakdown  
- Country-wise content production  
- Rating distribution among shows

**Challenges:**  
- Overlapping axis labels in time series charts reduced readability.  
- Pie charts with many categories became cluttered.

**Solutions:**  
- Rotated x-axis labels and limited tick marks for clarity.  
- Grouped smaller categories into “Other” to simplify pie charts.  
- Chose distinct color palettes to improve visual differentiation.

## 5. Overall Challenges and Learnings

Throughout the project, managing missing and inconsistent data was a significant challenge. Handling multi-valued categorical fields required careful parsing and transformation to allow meaningful analysis. Additionally, balancing detail and clarity in visualizations took iterative refinement.

This project reinforced the importance of thorough data cleaning and the value of exploratory visualizations in uncovering insights. It also provided practical experience working with real-world messy datasets and applying Python libraries to analyze and present data effectively.



