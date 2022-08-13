# School_District_Analysis

## Overview

The purpose of this challenge was to determine the extent to which the 9th grade scores from Thomas High School were disproportionately affecting the overall scores for that school and district. To accomplish this, we replaced all Thomas High School scores with scores from only 10th-12th graders at Thomas High School (i.e., substituting the 10th-12th grade scores for the complete 9th-12th grade scores), in order to identify how much the averages change by removing the 461 ninth-grade students from Thomas High School.

Completing this challenge involved identifying and comparing metrics in datasets containing information regarding student performance and school performance. The datasets include the student's year in school (9th through 12th), the name of the school the student attends, and their academic performance (math and reading grades), as well as information regarding each school's type (district or charter), number of students, and total budget. After merging a dataset containing school performance with a dataset containing student performance, we were able to quantify student performance against school-based metrics like the type of school and school budget. We then removed the Thomas High School 9th grade students in order to quantify the change after removal.


## Results

The overall result is that removing the Thomas High School ninth graders resulted in very little change to the averages calculated in the dataset. This is true for two reasons: the THS 9th graders' scores were very similar to THS 10th-12th graders' scores, and the population of THS ninth graders was very small (461) relative to the total number of students in the district (39,170), so the removal of THS ninth graders did not skew district-level metrics. 


- How is the district summary affected?
  - The district summary is affected only slightly because the population removed (ninth graders at one school) is small relative to the total population of students in the district. 

District Summary Before Removal of THS 9th Graders
![district summary PRE](https://user-images.githubusercontent.com/100863488/160855715-ef959cc3-2728-4a61-ae78-9cd077ae3099.png)

District Summary After Removal of THS 9th Graders
![district summary POST](https://user-images.githubusercontent.com/100863488/160855684-b66c80aa-6762-4b14-bceb-1f5c64f78be0.png)

- How is the school summary affected?
  - The THS school summary is affected only slightly, because the 9th graders' overall scores were very similar to scores of the rest of the THS student population. For example,
    - Average reading score for THS 9th graders: 83.73
    - Average reading score for THS 10th graders: 84.25

    - Average math score for THS 9th graders: 83.59
    - Average math score for THS 10th graders: 83.09

Per School Summary Before Removal of THS 9th Graders
![per school summary PRE](https://user-images.githubusercontent.com/100863488/160856040-38dcd433-f053-4396-b327-70cde6dbf746.png)

Per School Summary After Removal of THS 9th Graders
![per school summary POST](https://user-images.githubusercontent.com/100863488/160856006-60fdec4c-4245-4fe8-8948-5db64d020481.png)



- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
  - Replacing the 9th graders' scores did not meaningfully affect Thomas High School's performance relative to the other schools. The school rankings are not changed.




### How does replacing the ninth-grade scores affect the following:
  - **Math and reading scores by grade**

We replaced THS 9th grade math and reading scores with NaNs. Below are the math and reading scores by grade before replacing the 9th grade THS scores with NaNs. The 9th grade THS scores are very similar to other THS scores, and therefore the removal of 9th grade scores did not affect the averages significantly.

Math scores by grade:

![math scores by grade](https://user-images.githubusercontent.com/100863488/160856402-414aee0a-cd4d-4778-8829-bea743d4da4e.png)


Reading scores by grade:

![reading scores by grade](https://user-images.githubusercontent.com/100863488/160856462-b202c837-15a1-4bdf-8d2c-5dd83b3ca4cb.png)


  - **Scores by school spending**
    - Replacing the 9th graders' scores did not meaningfully affect Thomas High School's performance relative to the other schools. Thomas High School falls in the $631-$645 "spending per student bin," so between the initial analysis and the analysis omitting THS 9th graders, we would expect to see change only in that bin. The changes in scores are minimal.

Metrics by spending range before removal of THS 9th graders:
![spending ranges PRE](https://user-images.githubusercontent.com/100863488/160856769-10a8be65-56a2-4e6b-91cd-043c1dfb1c94.png)


Metrics by spending range after removal of THS 9th graders:
![spending ranges POST](https://user-images.githubusercontent.com/100863488/160856780-ca76bd18-a830-4f58-9d55-de43cf31237a.png)


  - **Scores by school size**
    - Replacing the 9th graders' scores did not meaningfully affect Thomas High School's performance relative to the other schools. Thomas High School, with 1,635 students, is a "medium size" high school for our purposes here, so we would expect to see changes only in that bin. The changes in scores are minimal.

Metrics by school size before removal of THS 9th graders:
![school size PRE](https://user-images.githubusercontent.com/100863488/160856886-99796e5d-434e-47dd-b09b-31e911c04628.png)


Metrics by school size after removal of THS 9th graders:
![school size POST](https://user-images.githubusercontent.com/100863488/160856919-0e3dc05d-aaa2-4ab9-8050-3f5ad4f863f9.png)


   - **Scores by school type**
     - Replacing the 9th graders' scores did not meaningfully affect Thomas High School's performance relative to the other schools. Thomas High School is a charter school, so we would expect to see changes only in that bin. The changes in scores are minimal.

Metrics by school type before removal of THS 9th graders:
![school type PRE](https://user-images.githubusercontent.com/100863488/160857081-194733c0-b026-430f-995d-ecd57e687c01.png)


Metrics by school type after removal of THS 9th graders:
![school type POST](https://user-images.githubusercontent.com/100863488/160857040-18b347be-26ff-4b22-a976-6868df637287.png)



## Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

On the whole, the changes were minimal. The Thomas High School 9th grade scores were very similar on the whole to Thomas High School scores in other grades, so removing the 9th grade scores did not change the overall metrics significantly. 

Four changes in the District Summary created by the removal of THS 9th grade scores were:
  - The average math score decreased from 79.0 to 78.9.
  - The percentage of students passing math decreased from 75.0% to 74.8%.
  - The percentage of students passing reading decreased from 85.8% to 85.7%.
  - The percentage of students who passed both math and reading ("Overall Passing") decreased from 65.2% to 64.9%.

