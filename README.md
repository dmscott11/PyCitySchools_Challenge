# PyCitySchools_Challenge
## Overview of PyCity Schools Analysis
The PyCity Schools analysis was originally completed to get a complete picture of the performance of schools within the school district. An issue arose where 9th grade students were found to have participated in academic dishonesty in some capacity. The school district requested that we re-complete the school district analysis but this time we exempt all 9th grade students from Thomas High School. This required re-factoring much of the code that was previously used and also allowed for the improvement of several lines of code. 
## Results of Analysis
The results of the analysis revealed that omitting the ninth-graders of Thomas High School affected several different measurements in minor ways. Overall, it can be seen in the charts that omitting ninth graders from Thomas High School lowered their test results dropping their overall passing percentage by roughly 0.3%. However, this was not enough to impact their rating among other schools in the school district. The results of these analysis can be seen in the following sections. 
### District Summary Changes
Due to the omisssion of roughly 400 students (9th Graders @ Thomas High) the overall scores of the district were seen to decline across every measurable category. The charts can be seen in both the Challenge code and the Original code with the list below explaining what exactly changed. The Challenge code omits the scores by 9th Graders at Thomas High while the Original code includes those scores. 
- Average math score decreased from 78.99 to 78.93.
- Average reading score decreased from 81.88 to 81.66.
- Passing math percentage decreased from 74.98% to 74.76%.
- Passing reading percentage decreased from 85.81% to 85.66%.
- Overall passing percentage decreased from 65.17% to 64.86%.
### School Summary Changes
Similarly to the District Summary, the changes in data occur from the grading and percentage measurements and in no other categories. There is no change in budget and money spent per student as it is the ninth-graders scores that are erased and not the ninth-graders as a whole. Therefore the student population does not change. 
### Thomas High School Relative Changes
Thomas High School did not drop any rankings by omitting the testing scores of ninth-graders. While their overall passing percentage did decrease, it was not enough to drop them from second overall to third. The percentage decrease was as follows:
- Original Overall Passing %: 90.95%
- New Overall Passing %: 90.63%
### Additional Charts
#### Math and Reading by Grade
Math and Reading were impacted by omitting those students as there were slight drops in overall scores. The drop itself does not apprea to be too significant with the largest decline occuring in Math and seeing a .22 drop in score.
#### Scores by School Spending
The changes in scores categorized by school spending were also minimal. 
These are the binned original scores:
![](/Images/speding_perstudent_before.png)

While these are the new scores by school spending:
![](/Images/spending_after.png)
#### Scores by School Size
This grouping did not provide much useful information. These groupings are too large to see any sort of meaningful change among scores or averages. 
Original:
![](/Images/schoolsize_before.png)

New:
![](/Images/schoolsize_after.png)
#### Scores by School Type
The scores by School Type analysis shows that there were no changes overall. This could be in part because of the quantity of students in each grouping. The loss of a few hundred students among thousands would have little impact on the average. 
Original:
![](/Images/schooltype_before.png)

New:
![](/Images/schooltype_after.png)
## Summation
In summation, it can be seen that the omitting of Thomas High Schools ninth-graders did decrease their overall scores, but it is difficult to tell whether this is from academic dishonesty. In order to more thoroughly understand whether academic dishonesty occurred, we would need to analyze all ninth-graders within the school district and come up with a ruling. The changes in overall school performance from Thomas High School are wrapped up in the following list:
- Average math score decreased from 78.99 to 78.93.
- Average reading score decreased from 81.88 to 81.66.
- Passing math percentage decreased from 74.98% to 74.76%.
- Passing reading percentage decreased from 85.81% to 85.66%.
- Overall passing percentage decreased from 65.17% to 64.86%.
### Additional Notes
One line of code that was extremely useful in formatting all #'s involved in this process was ``pd.options.display.float_format = '{:,.2f}'.format`` line which allowed me to bypass formatting in individual cells. 
