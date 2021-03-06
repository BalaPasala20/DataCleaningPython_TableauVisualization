# DataCleaningPython_TableauVisualization
A Museum's messy data about its objects is available in MessyData_Sample.csv. The goal is to clean the data and then visualize it using Tableau.

## Techniques used for data cleaning
* Identify the null values and their percentage to total values
* Remove null values when they are insignificantly small. The null values are removed for the string type data.
* Repetitive values with pipe delimiter are restructured to a single value within a data frame
* Data types of columns are changed appropriately.
* Medium column contains description about composition of objects in the museum. The word frequency is calculated within the column to identify different types of "Medium".
## Techniques used for Tableau visualization
* Text tables
* Horizontal bar charts
* Highlight tables
* Packed bubbles chart
## Prerequisites
* Jupyter notebook
* Tableau-desktop
## Steps to run the project
1. The python file "Clean_Data.ipynb" takes in "MessyData_Sample.csv" and outputs two .csv files - medium1.csv and Clean_Data.csv. The .csv files are also available in the repository.
2. After opening the Tableau desktop, the csv files - "medium1.csv" and "Clean_Data.csv" are taken as data source by a logical relationship by considering "Medium" as a common field. The worksheets are already developed to display the charts.

### Data Cleaning using Python:
1. "MessyData_Sample.csv" has messy data about the museum's objects.
2. The python program "Clean_Data.ipynb" takes the "MessyData_Sample.csv" and outputs two .csv files - "medium1.csv" and "Clean_Data.csv"
2. The columns - Object ID, Object Name, Medium, Department, Culture, Object Begin Date, Object End Data, and Artist Nationality, are considered for the analysis.
3. The "medium1.csv" contains the word frequency about each type of medium. The "Medium" column in "MessyData_Sample.csv" has description about composition of objects.
4. The "Artist Nationality" column has repetitve values with a pipe delimiter. A new column "Artist_Nationality_new" is created with a single value.
5. Clean data is saved inside "Clean_Data.csv".

### Outputs of Tableau visualization:
1. A calculated field "Age" is generated by finding the difference between "Object End Date" and "Object Begin Date".
2. Horinzontal bar chart showing different medium of artifacts in the museum.
3. Text table with a "Culture" filter showing "Department" of each "Object ID".
4. Text table with a bar chart showing average "age" of an "Object ID" under each "Culture" along with "Culture" filter.
5. Highlight table that displays no.of artists based on their nationality.
6. Horizontal bar chart showing top 20 oldest objects.
7. Packed bubble chart showing top "Culture"s that produced high number of "Object ID"s.

