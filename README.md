# School District Analysis

## Overview

A city school system chief data scientist has tasked us to do a complete analysis of various schools in a single district. The analysis is to help provide information for the district to determine how to assign budgets for the schools in the district. 

## Analysis
Upon initial inspection of the CSV file, there was a need for some cleanup in the student names. Various prefixes and suffixes had to be removed. Once the name cleanup was done, our first task was to removed Thomas High Schools math and reading scores, or rather replace them with a NaN. That in turn will change the overall numbers for Thomas' High School test scores.

### Adjusting Thomas High Schools Math and Reading Scores

once we've removed the 9th grade data sets of Thomas High School math and reading scores, we needed to recalculate the math, reading, and overall scores for the remaining grades. The inital data set looks as follows:

![Screen Shot 2021-04-11 at 16 04 07](https://user-images.githubusercontent.com/79731109/114321465-7e76d180-9ae0-11eb-9706-8c516541d014.png)

with the  change in Thomas High School data, the new data set looks as follows:

![Screen Shot 2021-04-11 at 16 04 23](https://user-images.githubusercontent.com/79731109/114321470-820a5880-9ae0-11eb-944f-c76ca0d51528.png)

By removing the 9th grade math and reading scores of Thomas High School, it brought up the passing rate for the district.

![Screen Shot 2021-04-11 at 15 57 37](https://user-images.githubusercontent.com/79731109/114321483-9189a180-9ae0-11eb-8f21-00600e70f0d3.png)

The changes to Thomas High Schools data set has propelled Thomas High School into one of the top 5 schools.

![Screen Shot 2021-04-11 at 16 15 30](https://user-images.githubusercontent.com/79731109/114321581-2a202180-9ae1-11eb-909e-471c69d1ef25.png)

### Looking at Spending Per Student

Once we've got that score changes taken care of,  we were tasked to take a look at the schools spending per student. Each schools budget differentiates on how much spending was for each student. So we had to categorize these by spending ranges.

![Screen Shot 2021-04-11 at 16 43 08](https://user-images.githubusercontent.com/79731109/114322308-065eda80-9ae5-11eb-8d89-ac5b1db13d6d.png)

looking at this data frame, those who have a higher spending on per student, have much lower grades than those who spend roughly about $630 per student and less.

### Looking at School Size

Much similar to how we did the spending ranges, we set up our code to look at the difference in school sizes.

![Screen Shot 2021-04-11 at 17 10 28](https://user-images.githubusercontent.com/79731109/114322995-d9acc200-9ae8-11eb-9c32-facb5c14f73b.png)

Schools that were considered small or medium were able to produce better grades than those of schools that were considered large

### Looking at Schools by Type

Finally we take a look at the correlation between grades and types of school.

![Screen Shot 2021-04-11 at 17 17 35](https://user-images.githubusercontent.com/79731109/114323683-eb439900-9aeb-11eb-8353-26efb9be6116.png)

Charter schools produced alot better scores than your average district school types.

## Summary

Overall, the change to Thomas High School's 9th grade scores did not effect the overall metrics of the schools by much. Schools that are more likely to succeed are schools that are around the mid to low range spending per students but with also a medium to small classes.
