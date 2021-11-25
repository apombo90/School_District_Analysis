# School_District_Analysis
## Project Overview
Analysis done for a School District to provide performance trends and patterns on student funding and students' standardized test scores based on school performance. This analysis attempts to assist the school board in making decisions regarding the school budgets and priorities. The analysis was done by completing the following tasks:

  1.  Creating a DataFrame with the district summary.
  2.  Creating a DataFrame with the school summary.
  3.  Identifying the Top 5 performing schools based on the overall passing rate.
  4.  Identifying the Bottom 5 schools based on the overall passing rate.
  5.  Calculating the average Math score for each grade level from each school.
  6.  Calculating the average Reading score for each grade level from each school.
  7.  Calculating the scores by school spending per student.
  8.  Calculating the scores by school size.
  9.  Calculating the scores by school type.

Finally, after performing this analysis I was notified that there was evidence of academic dishonesty for specifically, reading and math grades for Thomas High School ninth graders. As a result, the above tasks had to be repeated after replacing the altered data with NaNs. The results and project analysis are based in the comparison of the two versions of the data to describe how these changes affected the overall analysis.

## Resources
- Data source: schools_complete.csv, students_complete.csv
- Software: Python 3.7.10, Jupyter Notebook
## Results
- The District Summary wasn't highly affected by the updated analysis *(replacing the ninth graders’ math and reading scores of Thomas High School)* because the altered data represented 1.2% *(461 students with altered scores)* of the total data so it had a low impact on the average. Comparing both District Summaries, the data was impacted at a decimal level with the % Overall Passing having the highest impact decreasing by -0.3%.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;**District Summary without the altered data**
 
![image](https://user-images.githubusercontent.com/91766276/143324951-7e500c21-a03a-4406-bd2e-97504e11ea8c.png)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **District Summary including the altered data**

![image](https://user-images.githubusercontent.com/91766276/143325013-b1f51ca7-55e9-4b1a-9857-2d0d4e77377b.png)


- In the School Summary, clearly the school that was impacted with the new modified data was Thomas High School because the new analysis excluded this school's ninth graders scores, but the number of students remained the same in the data. The school went from having a 91% of the students passing both Math and Reading to a 65% on the updated analysis. 

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **School Summary without the altered data**

![image](https://user-images.githubusercontent.com/91766276/143328025-9ae838d1-5de5-45f7-8d61-8c351dd65802.png)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **School Summary including the altered data**

![image](https://user-images.githubusercontent.com/91766276/143328086-2fc81c90-0ff3-4105-a278-416893429ed9.png)

- Based on the previous problem with the Thomas High School performance having such a negative impact when updating the data, I performed a new calculation of this school's performance by calculating new metrics ignoring all its ninth graders students. That way the calculations were giving us the real school performance without the altered data. With this new calculation, the school kept its second place in the Top 5 performing schools.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Top 5 performing schools without the altered data**

![image](https://user-images.githubusercontent.com/91766276/143330360-b87e928c-1552-45d0-9e6e-b4f767c77ed6.png)

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; **Top 5 performing schools including the altered data**

![image](https://user-images.githubusercontent.com/91766276/143330062-fddab022-b0a9-490c-b4d2-4cb694ee85f7.png)

- Math and Reading scores were not affected by the new analysis, the only difference is that for Thomas High School the 9th grade score is NaN. The other schools where not impacted with the new updated analysis. 

![image](https://user-images.githubusercontent.com/91766276/143333161-62d1db2a-bbd5-47b9-ae8f-d289c2203096.png)

- The ***Scores by school spending, Scores by school size and Scores by school type*** were not affected by replacing the ninth graders scores for Thomas High School as the new scores were calculated without these students and their impact in the total data was very minimal. The advantage of having this new updated analysis is that the data remained consistent, and the "false" grades were excluded making the report more credible.

## Summary

The main changes that the school district analysis had after replacing the reading and math scores for Thomas High School's ninth graders where that the overall passing percentage for this school decreased by 0.3% and the average math score went from 79.0 to 78.9. Also, 461 students were removed from the District Summary as there was evidence of academic dishonesty in all 9th graders scores from THS, this reduced the total student count by 1.2%. Finally, we can determine that the impact on all other metrics was minimal, essentially Thomas High School kept its second place in the Top 5 performing schools.

