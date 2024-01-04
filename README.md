# pandas-challenge
Instructions
Using Pandas and Jupyter Notebook, create a report that includes the following data. Your report must include a written description of at least two observable trends based on the data.

Report Items:
1. Imported pandas & pathlib libraries.
2. Loaded csv files "schools_complete.csv" & students_complete.csv".
3. Stored the data into pandas DataFrames before combining them into one DataFrame. 
4. District Summary:
    - Used nunique(), sum(), mean(), count().
    - Calculated:Total Schools, Total Students, Total Budget, Average Math Score, Average Reading Score, % Passing Math, % Passing Reading, % Overall Passing.
5. School Summary:
    - Grouped the data by "school_name" using df.groupby.
    - Used count() & mean()
    - Calculaated (per school): School Type, Total Students, Per Student Budget, Average Math Score, Average Reading Score, % Passing Math, % Passing Reading, % Overall Passing.
6. Highest-Performing Schools (by % Overall Passing):
    - Used df.sort_values funcation to sort the School Summary by % Overall Passing in ascending order.
7. Lowest-Performing Schools (by % Overall Passing):
    - Used df.sort_values funcation to sort the School Summary by % Overall Passing in descending order.
8. Math Scores by Grade:
    - Seperated the math score data by grade and grouped by school_name.
    - Then combined the data into one DataFrame. 
9. Reading Scores by Grade:
    - Seperated the reading score data by grade and grouped by school_name.
    - Then combined the data into one DataFrame. 
10. Scores by School Spending:
    - Established spending bins & labels with dollar ranges. 
    - Used pd.cut to categorize the spending based on the established bins. 
11. Scores by School Size:
    - Established bins & labels based off school size (total students). 
    - Used pd.cut to categorize the school sizes based on the established bins.
12. Scores by School Type:
    - Grouped the school summary data by school type (Charter & District)
    - Calculated: Average Math Score, Average Reading Score, % Passing Math, % Passing Reading, % Overall Passing.
13. Summary analysis:
    - The top 5 performing schools are 100% Charter and the bottom 5 performing schools are 100% District. Based off of this alone, one can conclude that students perform better at Charter schools then at District schools. 
    - Other school characteristics that correlate with higher score metrics include smaller school size & smaller per student spending budget. Both of which, Charter schools tend to share, which could be the reason for the higher score metrics. 
    - Another notable observation, is that the average reading score for all schools is higher then the average math score. There isn't obvious reasons why this is within in the current data. But if we were to analyze school spending by subject, it would be interesting to see which subject has the largest spending. Especially because there seems to be a negative correlation between spending & performance.


Sources:
Data Bootcamp Class Recordings
https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.nunique.html
https://pandas.pydata.org/docs/reference/api/pandas.cut.html
https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.set_index.html
