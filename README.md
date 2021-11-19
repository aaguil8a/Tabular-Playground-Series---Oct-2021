# Student Math Performance

For this project, I took dataset from Kaggle about final scores of students at the end of a math programs with several features that might or might not impact the future outcome of these students. To that end, the following was asked when investigating this dataset: what factors influence students’ final grades in math course subjects? 


# Dataset

soure: https://www.kaggle.com/janiobachmann/math-students

* Entries: 395
* Features: 33
* Target: G3 (final grade numeric: from 0 to 20)


# Features:

Attributes for both student-mat.csv (Math course) and student-por.csv (Portuguese language course) datasets:

1 school - student's school (binary: 'GP' - Gabriel Pereira or 'MS' - Mousinho da Silveira)

2 sex - student's sex (binary: 'F' - female or 'M' - male)

3 age - student's age (numeric: from 15 to 22)

4 address - student's home address type (binary: 'U' - urban or 'R' - rural)

5 famsize - family size (binary: 'LE3' - less or equal to 3 or 'GT3' - greater than 3)

6 Pstatus - parent's cohabitation status (binary: 'T' - living together or 'A' - apart)

7 Medu - mother's education (numeric: 0 - none, 1 - primary education (4th grade), 2 â€“ 5th to 9th grade, 3 â€“ secondary education or 4 â€“ higher education)

8 Fedu - father's education (numeric: 0 - none, 1 - primary education (4th grade), 2 â€“ 5th to 9th grade, 3 â€“ secondary education or 4 â€“ higher education)

9 Mjob - mother's job (nominal: 'teacher', 'health' care related, civil 'services' (e.g. administrative or police), 'athome' or 'other') 10 Fjob - father's job (nominal: 'teacher', 'health' care related, civil 'services' (e.g. administrative or police), 'athome' or 'other')

11 reason - reason to choose this school (nominal: close to 'home', school 'reputation', 'course' preference or 'other')

12 guardian - student's guardian (nominal: 'mother', 'father' or 'other')

13 traveltime - home to school travel time (numeric: 1 - <15 min., 2 - 15 to 30 min., 3 - 30 min. to 1 hour, or 4 - >1 hour)

14 studytime - weekly study time (numeric: 1 - <2 hours, 2 - 2 to 5 hours, 3 - 5 to 10 hours, or 4 - >10 hours)

15 failures - number of past class failures (numeric: n if 1<=n<3, else 4)

16 schoolsup - extra educational support (binary: yes or no)

17 famsup - family educational support (binary: yes or no)

18 paid - extra paid classes within the course subject (Math or Portuguese) (binary: yes or no)

19 activities - extra-curricular activities (binary: yes or no)

20 nursery - attended nursery school (binary: yes or no)

21 higher - wants to take higher education (binary: yes or no)

22 internet - Internet access at home (binary: yes or no)

23 romantic - with a romantic relationship (binary: yes or no)

24 famrel - quality of family relationships (numeric: from 1 - very bad to 5 - excellent)

25 freetime - free time after school (numeric: from 1 - very low to 5 - very high)

26 goout - going out with friends (numeric: from 1 - very low to 5 - very high)

27 Dalc - workday alcohol consumption (numeric: from 1 - very low to 5 - very high)

28 Walc - weekend alcohol consumption (numeric: from 1 - very low to 5 - very high)

29 health - current health status (numeric: from 1 - very bad to 5 - very good)

30 absences - number of school absences (numeric: from 0 to 93)

these grades are related with the course subject, Math: 31 G1 - first period grade (numeric: from 0 to 20)

31 G2 - second period grade (numeric: from 0 to 20)

32 G3 - final grade (numeric: from 0 to 20, output target)


# Observation

Q1: What is the overall student performance?

![image](https://user-images.githubusercontent.com/55922514/142603999-d428eef2-7fa2-4b60-8dac-a55edb615775.png)

For the most part, students did not do that well since only 209 passed while 186 failed.


Q2: What are some factors that affect students’ final grades?


![download](https://user-images.githubusercontent.com/55922514/142604099-abe93126-a5f8-40dc-9568-830270eae6c7.png)

Q3: How much does absence influence students’ final grade?

![image](https://user-images.githubusercontent.com/55922514/142604282-cb14776f-83e3-49db-b4d3-8f5271188c6d.png)


We can see that given more absences, then students do worse in final grade.



Q4: How much does first grade and mid grades affect students’ final grade?

![download](https://user-images.githubusercontent.com/55922514/142604208-22ff84cf-04ef-49fd-bb10-7d2f4956c0ef.png)



![download](https://user-images.githubusercontent.com/55922514/142604226-58584c00-66ca-4e9d-b751-5fdb0d0a5a2a.png)

We see that if students do well in prior grading periods that will influence how well he/she does in final grades.

General observations: there are not many variables that show an influence on students’ final grades, which is interesting in itself since that may indicate the right kind of data was not gathered.

# Feature Importance

![image](https://user-images.githubusercontent.com/55922514/142604487-d3cde64e-b739-410e-a253-85daefa1c0af.png)




# Models Eva

![image](https://user-images.githubusercontent.com/55922514/142604546-595b4e21-b128-464b-b019-c84c3cce2cdb.png)

RF did best since it had the loweest prediction error.



