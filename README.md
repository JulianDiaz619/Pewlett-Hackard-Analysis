# Pewlett Hackard Analysis
An analysis based on retiring employees at "Pewlett Hackard"
## Purpose of Analysis
The main focus of this analysis was to see how many people are qualified to retire in order to allow the company to see how many people they should hire to replace retirees. I've included images to what I believe are the most important elements to our analysis.
## Results
* Creating Retirement Titles Table
* Creating Unique Titles Table
* Creating Retiring Titles Table
* Creating the Mentorship Program Eligibility Table
#### Retirement Titles Table
This analysis started off by creating a table based on employees born between 1952 and 1955. Here we had a lot of repeat values, so we had to further filter it down into our next table called "Unique Titles"
#### Unique Titles Table
We then filtered the retirement titles table using "DISTINCT" to ensure we only get one value of each employee, and further filtering it by only keeping values in which the "to_date" column is equal to '9999-01-01', which in our data, indicates that the employee has already left the company. Now that we have all unique values of employees who have retired, we need to count them, which is what we do in the "Retiring Titles" table.
![retirees](Pewlett-Hackard-Analysis/unique_table.png)
#### Retiring Titles Table
The retiring titles table we create allows us to make use of the unique titles table. Essentially we just a count of all our values in unique titles, so that we are able to see numerically just how many people in total left the company. 
![]()
#### Mentorship Program Eligibility Table
Now that we finished up seeing how many retirees the company has, we were instructed to create a table for employees eligible for a mentorship program.
