# School District Analysis

## Project Overview
A fictional Chief Data Scientist for a school district, Maria, was asked to analyze student funding and standardized test data. She asked for help to sort through the data, clense it, and uncover trends of school performance. After submitting our inital findings, Maria was notified that test scores at one of the schools may have been altered. She asked if we could remove the untrustworthy data and re-run our analysis before she presents the information to the school board.

The following information was gathered with and without the altered scores through analysis using Python: 

1. District Summary
2. School Summary
3. Top 5 Performing Schools (Overall Pass Rate)
5. Bottom 5 Performing Schools (Overall Pass Rate)
6. Scores by Grade and School
7. Scores by School Spending per Student
8. Scores by School Type

## Resources
Maria provided student data in a CSV file that contained each student's ID, name, gender, grade, school name, and standardized math and reading test scores. Additonally, she provided a seperate CSV that included each school's name, type, size, and budget. My approach was to analyze the CSV data using Python in a Jupyter Notebook, which allowed me to easily create dataframes and tables to showcase my findings. 
- Data Sources: students_complete.csv, school_complete.csv
- Software: Jupyter Notebooks 6.4.8
- Language: Python 3.7.13
- Libraries: Pandas, Numpy, os


## Results
The results below discuss the impact of excluding scores from 9th graders at Thomas High when compared to the original school district analysis.

### Impact on District Summary
Original District Summary: 
![Original District Summary](../main/Resources/district_sum_2.png)

Updated District Summary:
![Updated District Summary](../main/Resources/district_sum_1.png)

- Removing Thomas High's 9th grade reading and math scores did not have a significant impact on the district level summary. This view includes all students in the district, so removing the small portion of around 1% of all students only slighly changed the district level scores. All of the scores dropped by less than 0.3%, which leads me to believe that the excluded scores were not outliers significantly skewing the data. The scores excluded were; however, higher than the district's average, which is why the scores dropped slightly when excluded. 

### Impact on School Summary
Original Top 5 School Summary: 
![Original Top 5](../main/Resources/school_top_2.png)

Updated Top 5 School Summary:
![Updated Top 5](../main/Resources/school_top_1.png)

- Thomas High school remains the second top ranked school by overall passing percentage both before and after excluding the altered scores. 
- Thomas High school's data was the only row affected by the change, which makes sense because the excluded data only included student's from their school. It is worth nothing that their % Passing Reading and Overall Passing percentage descreased by 0.3%, which makes me believe the excluded data had a slightly higher percentages. 

Original Bottom 5 School Summary: 
![Original Bottom 5](../main/Resources/school_bottom_2.png)

Updated Bottom 5 School Summary:
![Updated Bottom 5](../main/Resources/school_bottom_1.png)

- The excluded data had not impact on the bottom school list. This is expected because Thomas High School was not on this list, which was the only school with data removed causing scores to change.

### Impact on Math and Reading Scores by Grade
Original Math Scores:

![Original Math Scores](../main/Resources/math_2.png)

Updated Math Scores:

![Updated Math Scores](../main/Resources/math_1.png)

Original Reading Scores:

![Original Reading Scores](../main/Resources/reading_2.png)

Updated Reading Scores:

![Updated Reading Scores](../main/Resources/reading_1.png)

- The updated reading and math scores both show a change in the score for THomas High 9th graders. When we initally included all data in the original code, we were able to calculate and return an average score for 9th graders at Thomas High. After excluding their data, the updated code had no data to calculate the average, so the dataframe shows "nan" to indicate there is no data avalible. 

### Impact on Scores by Spending
Original Scores by Spending: 
![Original Scores by Spending](../main/Resources/spending_2.png)

Updated Scores by Spending:
![Updated Scores by Spending](../main/Resources/spending_1.png)

- Thomas High is included in the $631-645 Spending Range, so this row was the only row for a potential impact to the summary data. We can see that the only differences between the two summary tables is a drop of 0.1% in the % Passing Reading and the % Overall Passing. The other metrics in the $631-645 Spending Range row were also impacted, but small enough that our level of rounding in the data table doesn't display it. 

### Impact on Scores by Size
Original Scores by Size: 
![Original Scores by Size](../main/Resources/size_2.png)

Updated Scores by Size:
![Updated Scores by Size](../main/Resources/size_1.png)

- Thomas High is included in the Medium Schoool Size range, so this row was the only row for a potential impact to the summary data. Comparing the two summary tables, we see the only metric impacted signficantly enough to show a difference in our table is a 0.1% decrease in the % Passing Reading, indicating the excluded students had a slightly higher passing percentage than the average Medium schools. 

### Impact on Scores by School Type
Original Scores by Type: 
![Original Scores by Type](../main/Resources/type_2.png)

Updated Scores by Type:
![Updated Scores by Type](../main/Resources/type_1.png)

- Thomas High is a Charter school, so we would expect to see the summary metrics for Charter schools change. In this case they actually did change, but the change was less than 0.1%, so there is no impact to our summary table due to the rounding format chosen. 


## Summary
After excluding the potentially altered reading and math scores for 9th graders at Thomas High School, the school district analysis changed in the following ways: 
1. The entire school district's overall pass rate decreased slightly by 0.3%, dropping from 64.9% to 65.2%. This indicates the students excluded had a higher overall pass % than the district average.
2. Thomas High School was originally ranked as the second highest performaing school in reference to overall pass percentage. After excluding the data, their pass rate decreased slightly, from 90.63% to 90.95%. However; they remained as the second highest ranked school. 
3. Excluding the data had a significant impact to the school summary analysis because the amount of student data excluded was the highest proportion to the population of Thomas High. One of the four grades at their school had data removed, which explains the slighlty larger impact of 0.3% drop in their reading and overall passing percentage.
4. The math and reading scores by grade table was notebly impacted - both tables had no data to calculate for Thomas High 9th graders in the updated run, so that value reads "nan" to indicate no results. 


