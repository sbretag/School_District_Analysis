# School District Analysis

## Overview of School District Analysis:

A school board and Maria have asked us to redo analysis on school and student performance due to evidence of academic dishonesty regarding reading and math scores for 9th graders at Thomas High School.  The following tasks and analysis have been requested.

1. Replace reading and math scores for 9th graders at Thomas High School with NaN
2. Repeat the school analysis excluding Thomas High School reading 9th grade reading and math scores
3. Provide a written summary on the impacts of excluding the scores in the analysis versus the original analysis

## Resources
- [School Data Source](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/schools_complete.csv)
- [Studen Data Source](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/students_complete.csv)
- Software: Jupyter Lab, Python 3.8.8

## Results

### Impact on District Summary

#### Original District Summary
![](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/Original_District_Summary.png)

#### New District Summary
![](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/New_District_Summary.png)

#### New vs Original District Summary
- No change to total schools, total students or total budget as only the scores were removed for Thomas High School (THS) 9th graders.  The students were still included in the total student count.
 - Average math and average reading scores dropped by 6 basis points (bps) and 2 bps respectively
 - % Passing Math and % Passing Reading dropped 22 and 15 bps resepectively
 - Overall passing % dropped by 31 bps
- Given the drop in all scoring categories, the scores removed were better than the overall district scores however the differences are fairly immaterial as the overall passing % rounds to 65% in both scenarios  

### Impact on School Summary


### Impact on Thomas High School's Performance Relative to Other Schools

#### Original School Summary (THS Only)
![New District Summary](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/Original_School_Summary_THS_Only.png)
[View Complete Original School Summary](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/Original_School_Summary.png)

#### New School Summary (THS Only)
![](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/New_School_Summary_THS_Only.png)
[View Complete New School Summary](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/New_School_Summary.png)

#### New vs Original School Summary
- No change to School Type, Total Students, Total School Budget, or Per Student Budget amounts.
 - 7 bps decrease in average math score
 - 5 bps increase in average reading score
 - 9 bps decrease in % passing math
 - 29 bps decrease in % passing reading
 - 32 bps decrease in overall passing %
- Based on the differences, the scores removes from the analysis were better than the average math score but worse than the average reading score.  Given the drop in passing %'s, it's also clear that had more passing for reading, math, and overall than the rest of the 10th, 11th, and 12th graders.
 

### Impact on Scores by Grade

#### Original Scores by Grade (THS Only)

##### Orig Reading Scores by Grade
![](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/Original_Reading_Scores_ByGrade_THS_Only.png)
[View Complete Reading Scores](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/Original_Reading_Scores_ByGrade.png)

##### Orig Math Scores by Grade
![](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/Original_Math_Scores_ByGrade_THS_Only.png)
[View Complete Math Scores](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/Original_Math_Scores_ByGrade.png)

#### New Scores by Grade (THS Only)

##### New Reading Scores
![](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/New_Reading_Scores_ByGrade_THS_Only.png)
[View Complete Reading Scores](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/New_Reading_Scores_ByGrade.png)

##### New Math Scores
![](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/New_Math_Scores_ByGrade_THS_Only.png)
[View Complete Math Scores](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/New_Reading_Scores_ByGrade.png)

#### New vs Original Scores by Grade
- The only difference is that 9th graders now show NaN in the new analysis for both math and reading scores which was the intent of this analysis

### Impact on Scores by School Spending

#### Original Scores by School Spending
![](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/Original_Scores_BySchool_Spending.png)

#### New Scores by School Spending
![](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/New_Scores_BySchool_Spending.png)

#### New vs Original Scores by School Spending
- Because the average spend per student for Thomas High School is $636, the only spending bucket impacted was the $630-$644 range
- For the $630-$644 range
  - Avg Math score reduced by 2 bps and avg reading score increased by 2 bps
  - % passing math reduced by 2 bps and % passing readying reduced by 7 bps
  - Overall passing % reduced by 8 bps
- Overall, removing THS 9th grader scores does not result in a different story when it comes to spending by student, there does not appear to be relationship between more spending and higher scores, if anything, it's opposite.

### Impact on Scores by School Size

#### Original Scores by School Size
![](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/Original_Scores_BySchool_Size.png)

#### New Scores by School Size
![](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/New_Scores_BySchool_Size.png)

#### New vs Original Scores by School Size
- Because the size of Thomas High School is in the medium size group, the only size bucket impacted was the 1,000-2,000 range
- For the medium size schools
  - Avg Math score reduced by 1 bps and avg reading score increased by 1 bps
  - % passing math reduced by 2 bps and % passing readying reduced by 6 bps
  - Overall passing % reduced by 6 bps
- Overall, removing THS 9th grader scores does not result in a different story when it comes to school size, medium size schools continue to have the best passing %'s, they also continue to remain just behind small size schools in average scores.


### Impact on Scores by School Type

#### Original Scores by School Type
![](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/Original_Scores_BySchool_Type.png)

#### New Scores by School Type
![](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/New_Scores_BySchool_Type.png)

#### New vs Original Scores by School Type
- Because Thomas High School is a charter school, there is only an impact to the charter school category
- For charter schools
  - No material change to average math or reading scores
  - % Passing math reduced by 1 bps
  - % Passing reading reduced by 4 bps
  - % Overall passing reduced by 4 bps
- Overall, removing THS 9th grader scores does not result in a different story when it comes to school type, passing %'s remain significantly higher for charter schools than non charter schools


### Impact on Top 5 Status

#### Original Top 5 Schools
![](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/Original_Scores_BySchool_Type.png)

#### New Top 5 Schools
![](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/New_Scores_BySchool_Type.png)

#### New vs Original Top 5 Schools


## Summary

SUmmarize four changes in the updated school district analysis after reading and math scores for the ninth grade at THomas High School have been replaced with NaNs


