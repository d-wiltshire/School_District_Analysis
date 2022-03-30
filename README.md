# School_District_Analysis

## Overview of the school district analysis: Explain the purpose of this analysis. 

The purpose of this challenge was to determine the extent to which the 9th grade scores from Thomas High School were disproportionately affecting the overall scores for that school and district. The goal of the challenge was to replace all Thomas High School scores with scores from only 10th-12th graders at Thomas High School (i.e., substituting the 10th-12th grade scores for the complete 9th-12th grade scores), in order to identify how much the averages change by removing that one set of scores (i.e., removing the 461 ninth-grade students from Thomas High School).

Completing this challenge involved identifying and comparing metrics within two datasets containing information regarding student performance and school performance. The datasets include the student's year in school (9th through 12th), the name of the school the student attends, and their academic performance (math and reading grades), as well as information regarding each school's type (district or charter), number of students, and total budget. After merging these two datasets, we were able to quantify student performance against school-based metrics like the type of school and school budget. 


## Results: Using bulleted lists and images of DataFrames as support, address the following questions.

The overall result is that removing the Thomas High School ninth graders resulted in very little change to the averages calculated in the dataset. This is true for two reasons: the THS 9th graders' scores were very similar to THS 10th-12th graders' scores, and the population of THS ninth graders was very small (461) relative to the total number of students in the district (39,170), so the removal of THS ninth graders did not skew district-level metrics. 


### How is the district summary affected?

The district summary is affected only slightly because the population removed (ninth graders at one school) is small relative to the total population of students in the district. 

(screenshots - done)


### How is the school summary affected?

The THS school summary is affected only slightly, because the 9th graders' overall scores were very similar to scores of the rest of the THS student population. For example,

- Average reading score for THS 9th graders: 83.73
- Average reading score for THS 10th graders: 84.25

- Average math score for THS 9th graders: 83.59
- Average reading score for THS 10th graders: 83.09

-check these and add other scores



### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Replacing the 9th graders' scores did not meaningfully affect Thomas High School's performance relative to the other schools.

add per school summary screenshot

Please note that the "average reading score" and "average math score" were not adjusted between these two calculations.


### How does replacing the ninth-grade scores affect the following:
#### Math and reading scores by grade

(add screenshots of math and reading scores)

#### Scores by school spending
Replacing the 9th graders' scores did not meaningfully affect Thomas High School's performance relative to the other schools. Thomas High School falls in the $631-$645 "spending per student bin," so between the initial analysis and the analysis omitting THS 9th graders, we would expect to see change only in that bin. The changes in scores are minimal.

(add screenshots of pre and post spending)

#### Scores by school size
Replacing the 9th graders' scores did not meaningfully affect Thomas High School's performance relative to the other schools. Thomas High School, with 1,635 students, is a "medium size" high school for our purposes here, so we would expect to see changes only in that bin. The changes in scores are minimal.

(add screenshots of pre and post school size)

#### Scores by school type
Replacing the 9th graders' scores did not meaningfully affect Thomas High School's performance relative to the other schools. Thomas High School is a charter school, so we would expect to see changes only in that bin. The changes in scores are minimal.

(add screenshots of pre and post school type)



## Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

On the whole, the changes were minimal. The Thomas High School 9th grade scores were very similar on the whole to Thomas High School scores in other grades, so removing the 9th grade scores did not change the overall metrics significantly. 

-list changes from the above screenshots

