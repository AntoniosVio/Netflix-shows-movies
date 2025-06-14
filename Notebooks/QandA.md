# Netflix Data Analysis Project — Q&A Sheet

**1. Why did you choose this dataset?**  
I chose the Netflix Titles dataset because it provides a rich source of information about a popular streaming platform’s content. It allows exploration of trends in media type, ratings, release years, and durations, making it ideal for practicing ETL, data cleaning, and visualization skills.

**2. What were the main challenges in cleaning the data?**  
The dataset had inconsistencies such as missing values, mixed data types, and irregular formatting (e.g., ‘date_added’ field). Duration was stored as text with units (like “90 min”), requiring extraction and conversion to numeric. Handling these ensured accurate analysis.

**3. How did you handle missing or inconsistent data?**  
I identified missing values and decided on appropriate strategies—either removing rows with critical missing data or imputing with defaults where reasonable. I also standardized date formats and extracted numeric values from text fields to maintain consistency.

**4. What insights did your visualisations reveal?**  
The heatmap showed little correlation between numeric fields, suggesting independent variables. The scatter plot revealed a rise in movie durations over recent years. The pie chart highlighted that most titles are adult-rated (‘TV-MA’, ‘TV-14’), showing Netflix’s content focus.

**5. Why did you choose these specific charts?**  
Heatmaps are great for spotting correlations, scatter plots for trend analysis over time, and pie charts for distribution breakdowns. These visualizations clearly communicate different aspects of the dataset in an accessible way.

**6. Were there any surprising findings?**  
I found that despite a growing number of releases, movie durations vary widely with no strict pattern. Also, TV shows lack uniform duration data, reflecting varied episode lengths and formats.

**7. How could this analysis be expanded or improved?**  
Future work could include genre-based analysis, regional availability differences, viewer ratings integration, or sentiment analysis of reviews. Also, exploring more advanced machine learning models could predict content popularity.

**8. What tools and libraries did you use, and why?**  
I used Python with pandas for data manipulation, seaborn and plotly for visualisations due to their flexibility and aesthetics, and Git/GitHub for version control and collaboration.

**9. How did you ensure your code is reproducible and maintainable?**  
I wrote clear, well-commented code, used consistent file naming, and documented the ETL steps in both code comments and README. The use of version control ensures tracking changes and collaborative development.

**10. What limitations does your analysis have?**  
The dataset lacks viewer engagement metrics, which limits insights on content popularity. Some fields have missing or inconsistent data that could bias results. The analysis focuses on descriptive statistics without predictive modelling.
