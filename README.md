# School_District_Analysis

## 1. Overview of the school district analysis project

Maria is Chief Data Scientist  for the City School District. She is responsible for analysing data and provide insights for the board to take strategic decisions. In this project, Maria has asked us to go deeper in the data in order to analyse student funding and student test scores and identify trends. 

After a first round of analysis, the school board has notified Maria that the database we already worked on shows evidence of academic dishonesty. It appears that the reading and math grades from Thomas High School had been altered. In order for the board to be able to uphold state-testing standards, they have asked us not to include some test results from this school in the database. Though Maria has asked us to replace the math and reading scores from Thomas High School with NaNs while keeping the rest of the data intact. Then we will repeat the school district analysis with the new data and present our findings regarding the impact of these changes on the overall analysis.

## 2. Major findings regarding the school district performances

### 2.1 Impacts on the district summary
The impact of the changes we made regarding the Thomas HS performances is really limited. The average math score becomes 78.9 instaed of 79 and the average reading score is identical (81.9). If we format the percentage passing scores with two decimals, we highlight a slightly lower performances in reading and math (see the results in the tables below).

Full District summary analysis 
  
![District_summary](https://user-images.githubusercontent.com/85641189/125441170-7f77a564-73e3-4916-95e6-9b9d63fd08d6.png)

District summary whithout the 9th graders performances from Thomas HS
  
![District_summary_adjusted](https://user-images.githubusercontent.com/85641189/125441265-df378ed2-d1fa-4594-91d5-f50db17e73ad.png)

### 2.2 Impacts on the school summary
The school summary is affected on the results regarding the Thomas High School. In comparison with the analysis we did before, we have only changed the calculation for the performances of Thomas High School. Instead of considering all the sutdents from grande 9th to 12th, we have limited our analysis on the students from grande 10th to 12th. The overall results (average results and percentages) for this school are affected.
However, we have to highlight to the board that the difference between the results is really limited. We have to format the data with two decimals to be able to determine the impact on the school summary and the Thomas HS performances. For instance, the overall percentage of students passing math and reading is 90.63 in comparison with 90.94 if we consider all the students from Thomas High School.

### 2.3 Impacts on Thomas High School performances
Thomas High School is ranked second in the district schools, whatever the database we consider. Even if the performances of the students are slightly lower when we do not consider the 9th graders, the school performances are still really good and the school keeps is second place in the chart.

Top five schools performances

![Top_schools](https://user-images.githubusercontent.com/85641189/125450807-cbb83017-0810-497a-8dc0-ecb65701a170.png)

### 2.4 How does replacing the 9th graders scores affect the following:
  * math and reading scores by grade: only the 9th grade scores from Thomas High School are affected by the new analysis. The result appears as 'NaN' because we remove all the data in the database and we replace it by 'NaN'. See below the chart for the math score by grade for the fifteen schools from the district.

![Math_score_grade](https://user-images.githubusercontent.com/85641189/125455585-213ca4ce-03f6-4453-bea6-20ed40e198d2.png)

  * scores by school spending: replacing the 9th graders score by 'NaN' lower the average scores on math and reading for the schools spending between $630 and $644 because Thomas High School is in this category. The table below registers the modified results and we have written with a red pen the results from the first analysis we did.

![Score_spending_modified](https://user-images.githubusercontent.com/85641189/125482165-1e3287ee-18b5-4cae-8683-e1235da880ac.png)

  * scores by school size: replacing the 9th graders score by 'NaN' modified slightly the score by school size for the medium category because Thomas High School is in this category. 

![Score_size_modified](https://user-images.githubusercontent.com/85641189/125480847-a7ccaf02-0834-45fd-a582-f752b192da12.png)

It is important to notice that the school ranking based on percentage of students passing the math test is modified. The medium size schools register higher proportion of students passing the math test, whereas the small size schools used to be on the top.    

  * scores by school type: replacing the 9th graders score by 'NaN' modified slightly the score for the charter schools category because Thomas High School is in this category. 

![Score_type_modified2](https://user-images.githubusercontent.com/85641189/125480571-5a16856e-13e8-40a2-a77d-de436868760e.png)
 
## 3. Highlighting four changes on the updated school district analysis

### 3.1 Reducing the total number of students passing the tests
Replacing the 9th graders score by 'NaN' changes the number of students passing the math test with a score above 70. The total number of students passing the math test is 28,939 in the updated analysis whereas it was 29,370 during our first analysis.
This update has the same impact on the total number of students passing the reading test with a score above 70. The total number of students passing the reading test is 33,158 in the updated analysis (33,610 students in the first analysis).

![Math_passing_students_modified](https://user-images.githubusercontent.com/85641189/125484733-271a0534-8cf7-4a52-a08b-0b2e4c5429ef.png)

The overall result is also impacted with 25,105 students passing the math and the reading test whereas we had 25,528 students in our first analysis.

### 3.2 Reducing the percentage of students passing the tests
This reduced number of students passing the test, either math or reading, has slightly lowered the metrics "% Passing math", "% Passing reading", and "% Overall passing". Please find below the explanation of the calculation to understand the impact on the analysis. We will consider the calculation for the percentage of students passing the math test. To do this calculation, we have to consider the students who have a math score equal or above 70. Because we do not consider the 9th graders, this total is lower than the total in our first analysis. Then we have divided this score by the updated total of students, which is also lower. 

![%Passing_math_calculation](https://user-images.githubusercontent.com/85641189/125489169-8024a0f1-16e7-4670-9070-d82c118bdc3a.png)


Our overall recommandation is that the presomption of academic dishonesty does not have impacted so much the school district analysis we did first. If the school performances for Thomas High School is a bit lower in the updated analysis, the overall analysis of the metrics is not changed. Thomas High School, even whithout the 9th graders results, is still in the top five of the schools in the district. 


