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
![retirees](/unique_table.png)
#### Retiring Titles Table
The retiring titles table we create allows us to make use of the unique titles table. Essentially we just count of all our values in unique titles, so that we are able to see numerically just how many people in total left the company. 

![count](/unique_retiring.png)

Query that creates unique titles, then counts the total for each title.

![retirees](/retiring_table.png)

This table has the most vital information in our analysis I believe. What this table tells us is the total amount of retirees by title, which tells us how many of each title need to be hired.
#### Mentorship Program Eligibility Table
Now that we finished up seeing how many retirees the company has, we were instructed to create a table for employees eligible for a mentorship program.
![mentorship](/mentorship_table.png)
## Summary 
How many roles need to be filled after the "silver tsunami?". Referring to the Retiring Titles table, we can see a total of 25916 Senior Engineers, 24926 Senior Staff, 9285 Engineers, 7636 Staff, 3603 Technique Leaders, 1090 Assistant Engineers, and 2 Managers need replacing. Quite a lot of people!

Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
![](/mentorship_total.png)

Here is a query that might help us solve this question. The corresponsing table looks like this.

![](/mentorship_total_table.png)

I think the ratio is quite large from employees that need to be hired compared to the employees that are eligible for the mentorship program, but as long as they have a good training program I think the newcoming employees won't have too hard of a time adjusting to the company, also considering the majority of people that need to be hired are Senior Engineers, it implies that they already have a lot of experience with their job .
