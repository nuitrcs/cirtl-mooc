# Data Files

Files contain all the data necessary to reproduce the plots and analysis in both the main paper and the Supplemental Information. Fields have been removed to protect the anonymity of the participants. Some fields have been modified to remove extraneous information or protect anonymity. The data files are categorized as follows:

## Enrollment and Course Activity
1. `enrollments_pub.csv`: Summarized course activity for each participant in the seven instances of the introductory course. 
2. `enrollments_adv_pub.csv`: Summarized course activity for each participant in the four instances of the advanced course.

The enrollment tables contain the following fields:
* _activity_pga[i]_: [boolean] Attempted Peer-Graded Assessment i.
* _activity_q[i]_: [boolean] Attempted Quiz i.
* _activity_vid_count_: [integer] Total number of unique videos watched.
* _activity_vid_week_[i]: [integer] Number of unique videos watched from Module i.
* _course_platform_: [COURSERA|EDX] The MOOC platform for the course instance.
* _course_name_: [string] Name of the course instance
* _activity_completed_: [boolean] Completed the course by receiving a passing grade.
* _activity_learner_: [boolean] Met the criteria for "Learner" as defined in the paper.
* _activity_auditor_: [boolean] Met the criteria for "Auditor" as defined in the paper.
* _unique_user_id_: [string] Unique ID used to link surveys and enrollment data

## Pre-course survey
3. `pre_survey_pub.csv`: Pre-course survey responses.
4. `pre_survey_demo_pub.csv`: Pre-course survey respondent genders; separated from other responses for IRB compliance. 
5. `pre_survey_question_info.csv`: Pre-course survey question metadata.
6. `pre_survey_country_counts.csv`: Table of the number of participants representing each country of origin in each course course instance, determined from pre-survey responses.

The `pre_survey_pub.csv` table contains the following columns:
* _unique_user_id_: [string] Unique ID used to link surveys and enrollment data.
* _course_name_: [string] Name of the course instance
* _course_platform_: [COURSERA|EDX] The MOOC platform for the course instance.
* _QID[xxx]_: Pre-survey questions. Descriptions and meta-data for each survey question are given in `pre_survey_question_info.csv`.

## Post-course survey
6. `pst_survey_pub.csv`: Post-course survey responses.
7. `pst_survey_demo_pub.csv`: Post-course survey demographic responses; separated from other responses for IRB compliance.
8. `pst_survey_question_info.csv`: Post-course survey question metadata.

The `pst_survey_pub.csv` table contains the following columns:
* _unique_user_id_: [string] Unique ID used to link surveys and enrollment data.
* _course_name_: [string] Name of the course instance
* _course_platform_: [COURSERA|EDX] The MOOC platform for the course instance.
* _QID[xxx]_: Pre-survey questions. Descriptions and meta-data for each survey question are given in `pst_survey_question_info.csv`.
