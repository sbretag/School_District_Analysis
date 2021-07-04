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

### District Summary

![](https://github.com/sbretag/School_District_Analysis/blob/main/Resources/District_Summary_Comparison.png)



[Terminal Output of Audit Results](https://github.com/sbretag/Election_Analysis/blob/main/Analysis/Election_Results_TerminalOutput.png)

#### Original vs New School Summary Analysis


### School Summary





## Summary
Overall, the results of the audit were collected in an accurate and efficient manner using python code.  Given the success, we would like to propose handling all future election audits in both states and nationally.  The script used to perform an audit in this election is flexible and with minor modifications it can handle other types of elections with the same success.  Here are a few examples:
  1. Assuming the source data is available, we could provide more granuluar audit results by zip code by adding a new list for zip codes and creating votes by zip code dictionary.  By running through a similiar script as we did for county results, we could provide an output of vote count by zip code and zip code votes as % of overall total.
  2. For election results that have more than one type of race such as the house and senate, we could expand the script to include a list of the different races and a dictionary with a the candidates associated with each race.  In addition to adding data structures, a new for loop would need to be added to go through all of the different races and a condition would need to be added to filter on the candidates only associated with the particular race that's being analyzed in the for loop. 
  
