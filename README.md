# School_District_Analysis

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
- Data Source: students_complete.csv, school_complete.csv
- Software: Jupyter Notebooks
- Language: Python
- Libraries: Pandas, Numpy, os


## Results

### Impact on District Summary
Original District Summary: 
![Original District Summary](../main/Resources/district_sum_1.png)

Updated District Summary:
![Updated District Summary](../main/Resources/district_sum_2.png)

- Removing 

### Impact on School Summary
Original Top 5 School Summary: 
![Original Top 5](../main/Resources/school_top_1.png)

Updated Top 5 School Summary:
![Updated Top 5](../main/Resources/school_top_2.png)

- Removing 

Original Bottom 5 School Summary: 
![Original Bottom 5](../main/Resources/school_bottom_1.png)

Updated Bottom 5 School Summary:
![Updated Bottom 5](../main/Resources/school_bottom_2.png)

- Removing 

### Impact on School Summary
Original Top 5 School Summary: 
![Original Top 5](../main/Resources/school_top_1.png)

Updated Top 5 School Summary:
![Updated Top 5](../main/Resources/school_top_2.png)

- Removing 


## Summary
After excluding the potentially altered reading and math scores for 9th graders at Thomas High School, the school district analysis changed in the following ways: 
1. th 
2. th
3. th
4. th




```
# Add a variable to load a file from a path.
file_to_load = os.path.join("Resources", "election_results.csv")
# Add a variable to save the file to a path.
file_to_save = os.path.join("analysis", "election_analysis.txt")
```
