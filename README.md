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
Maria provided data in a CSV file that contained each student's ID, name, gender, grade, school name, and standardized math and reading test scores. My approach was to analyze the CSV data using Python in a Jupyter Notebook, which allowed me to easily create dataframes and tables to showcase my findings. 
- Data Source: students_complete.csv
- Software: Python 3.9.12, Jupyter Notebooks

## Results
The analysis of the election by county show that: 
- Effect on District Summary
- Effect on School Summary


## Summary
The output of this script contains accurate statstical data that can be used to determine the winner of any election along with voter turnout data by county. If the results file format is changed, your team can easily fix the code to continue to work. Additonally, this script may be easily used by your team to audit future elections, whether they are at the local level or have a larger data set, such as the state level. The script may also be modified to extract and summarize additonal data about voters and the votes recieved.

### Input File Column Order


```
# Add a variable to load a file from a path.
file_to_load = os.path.join("Resources", "election_results.csv")
# Add a variable to save the file to a path.
file_to_save = os.path.join("analysis", "election_analysis.txt")
```
