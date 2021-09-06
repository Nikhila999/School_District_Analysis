# School_District_Analysis

## Overview of the School District Analysis

In this project we are working with the student funding and student standardized test scores data. Based on the analysis and insights we provide, the school board will make strategic decisions and set priorities for all the schools in the district.  

### Purpose of this analysis
The school board has informed about the academic dishonesty in Math and Reading scores provided by Thomas High School for 9th grade. We do not have more details on the range of duplicity, so for our analysis we are replacing all the math and reading scores for 9th grade Thomas High School values with NaN (Not a Number). This will exclude the data from results.

## Results

1. How is the district summary affected?
    - After replacing the Math and Reading scores for Thomas High School, 9th grade students with NaNs (Not a Numbers), there is not a significant difference in the district summary values. The difference is negligible around 0.2% points.

2. How is the school summary affected?
    - We have calculated the Thomas High School summary two ways,
    1. First, we have replaced the Thomas High School, 9th grade Math and Reading scores with NaNs. Because we are replacing the math and reading score values with NaN, the total number of students in the school include 9th-12th grades, 1635 students and their %Passing Math, %Passing Reading and %Overall Passing are, 66.9%, 69,7% and 65.1% respectively.
    -- add replacing 9th grade pic
    
    2. In the second scenario, we have ignored Thomas High School 9th grade records (we are considering the total number of students from 10th-12th). To calculate the %Passing values, we are removing the 461 students from 9th grade and considering only 1174 students from 10th-12th grade. %Passing Math, %Passing Reading and %Overall Passing are, 93.2%, 97.0% and 90.6% respectively
    -- add removing 9th grade pic

3. How does replacing the ninth grader's math and reading scores affect Thomas High School's performance relative to the other schools?
    - Replacing the 9th grade values with NaNs has not had notable difference, however removing the 9th grade records have improved the percentage passing significantly, from the pictures above we can see that the passing percentages have jumped from less than 70% to greater than 90%.

4. How does replacing the ninth-grade scores affect the following
    - Math and reading scores by grade
        - Thomas High School, 9th grade math and reading scores are diplayed as nan, because we have replaced the record values as NaN.
    - Scores by school spending
        - There is no difference in school spending after replacing the 9th grader's math and reading score to NaN, because the per_school_capita is the same. If we were to remove the Thomas High School 9th grade records from the dataset, we would have seen the difference in scores by school spending.
    - Scores by school size
        - There is no difference in school size after replacing the 9th grader's math and reading score to NaN, because the total students in the school is same. If we were to remove the Thomas High School 9th grade records from the dataset, we would have seen the difference in scores by school size.
    - Scores by school type
        - There is no difference in school type after replacing the 9th grader's math and reading score to NaN, because the school type is the same. Even if we are to remove the Thomas High School 9th grade records from the dataset, we would not have seen any difference in scores by school type because, Thomas Hogh School is a Charter school.
        
## Summary

After chainging the math and reading scores with NaNs for Thomas High School 9th grade, we noticed that:
1. The school summary metrics have changed the most. We calculated the school summary with total number of students including 9th grade and exclusing 9th grade students. 
    When we excluded the 9th grade students records, the math, reading and overall percentages have poped significantly compared to just replacing the scores with NaNs.
2. There is a slight difference in the district summary metric values.
3. In Scores by grade metric, we are seeing that Thomas High School 9th grade, math and reading value is displayed as nan, because we updated the record.
4. There is no difference in scores by school spending, scores by school size and scores by school type metrics, because we are replacing the score value with NaN but not remvoing the record.
    


