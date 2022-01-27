# School_District_Analysis

## Overview

Analysing the school and student data with python using panda in Jupyter Notebooks.

### Purpose

The purpose is to create the following for the school district:
  - A high-level snapshot of the district's key metrics, presented in a table format.
  - An overview of the key metrics for each school, presented in a table format.
  - Tables presenting each of the following metrics:
    - Top 5 and bottom 5 performing schools, based on the overall passing rate.
    - The average math score received by students in each grade level at each school.
    - The average reading score received by students in each grade level at each school.
    - School performance based on the budget per student.
    - School performance based on the school size.
    - School performance based on the type of school.

### Resources

- Data Source
  - [schools_complete.csv](https://github.com/tkiruthika/School_District_Analysis/files/7944467/schools_complete.csv)
  - [students_complete.csv](https://github.com/tkiruthika/School_District_Analysis/files/7944470/students_complete.csv)
- Software
  - Jupyter Notebook

## School District Analysis

To start our analysis
  - First we cleaned the prefixes and suffixes in student name in the student data set using **str.replace()** function.
  - Then we checked the dataset for null values using **isnull()**.
  - Merge the two datasets into a single data set with **merge()**.
  - Average reading and math scores are calculated using **mean()**.
  - The **count()** is used to get the total number of students and the number of schools in the district.
  - The conditionals **&** and **>=** are used to find passing students in math, reading and in both.
  - The average scores and percentage values are formatted using **map()** and the school district summary dataframe is printed.
  - Using the **set.index()** the school performance is analysed accoring to the size, type, and budget(Spending scores).
  
## Challenge
  
  It was said that there is a academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appears to have been altered. So, we are asked to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. After replacing we need to repeat the school district analysis.

To start the challenge, we replaced the math and reading scores of Thomas High School, Ninth graders to Nan using **np.Nan**. After replacing, all the analysis functions are performed on the data set and the results are displayed.
  
## Results

  - **District Summary**
  
  The District summary of the school data set before replacing the math and reading scores of Thomas High School, Ninth graders to Nan.

  ![1](https://user-images.githubusercontent.com/95719819/151432362-56417a71-7b23-438c-9dfd-969d5e85438a.png)
  
  The District summary of the school data set after replacing the math and reading scores of Thomas High School, Ninth graders to Nan.
  
  ![2](https://user-images.githubusercontent.com/95719819/151430959-b0ea3a3d-795a-4ee2-ae89-cf344e2b39a4.PNG)

  - **School Summary**
  
  The school summary of the school data set before replacing the math and reading scores of Thomas High School, Ninth graders to Nan.
  
  ![ss1](https://user-images.githubusercontent.com/95719819/151431458-5d1101a6-bc05-4fe4-89fe-02ab227f1209.PNG)
  
  The school summary of the school data set after replacing the math and reading scores of Thomas High School, Ninth graders to Nan.

  ![ss2](https://user-images.githubusercontent.com/95719819/151431489-ae56ab25-c2a3-4772-afdc-98cf242998b9.PNG)

  - **Thomas High School’s performance with the new student count**
  
  The school summary of the school dataset after subtracting the number of ninth graders students in Thomas High School from the total student count.
  
  ![3](https://user-images.githubusercontent.com/95719819/151431542-e949f9a9-aa89-4662-bb56-351a1f63666f.PNG)
  
  - **Top 5 performing schools, based on the overall passing rate**
  
  The top 5 performing schools before replacing the ninth graders score in Thomas High School.
   
  ![top 5](https://user-images.githubusercontent.com/95719819/151431673-66ae177b-9b8a-4f98-a20a-e7cd1344d6fc.png)
  
  The top 5 performing schools after replacing the ninth graders score in Thomas High School.
  
  ![top5_c](https://user-images.githubusercontent.com/95719819/151431677-18552280-7365-445e-a10f-2d96dec9e9a3.PNG)

  - **Bottom 5 performing schools, based on the overall passing rate**
  
  The bottom 5 performing schools before replacing the ninth graders score in Thomas High School.
  
  ![bottom5](https://user-images.githubusercontent.com/95719819/151431816-c8d3f9c6-e63e-4e0e-923b-42759c69cf09.PNG)
   
  The bottom 5 performing schools after replacing the ninth graders score in Thomas High School.
  
  ![bottom5_c](https://user-images.githubusercontent.com/95719819/151431775-8c103353-1ebd-4bf1-b23c-f7e465a1c480.PNG)

  - **Math scores by grade**
  
  Math scores by grade before replacing the ninth graders score in Thomas High School.
  
  ![math1](https://user-images.githubusercontent.com/95719819/151432839-7d07dccb-c5fa-46bb-99bd-e6b76f6cc40b.PNG)
  
  Math scores by grade after replacing the ninth graders score in Thomas High School.
  
  ![math scores](https://user-images.githubusercontent.com/95719819/151265959-a4903810-23a2-44f8-bc12-1aa3b43f5518.PNG)
  
  - **Reading scores by grade**

  Reading scores by grade after replacing the ninth graders score in Thomas High School.
  
  ![reading1](https://user-images.githubusercontent.com/95719819/151432937-5118a865-2b8f-4d3a-9990-133b49d22ded.PNG)
  
  Reading scores by grade after replacing the ninth graders score in Thomas High School.
  
  ![reading scores](https://user-images.githubusercontent.com/95719819/151265977-5c3b8f6c-0c4c-43fb-8187-086f86eda11c.PNG)

  - **Scores by school spending**

  Spending score of Thomas High School before replacing the ninth graders score.
  
  ![spending1](https://user-images.githubusercontent.com/95719819/151433547-7ed0e3f5-e7ea-4c15-b8d8-973695373383.PNG)
  
  Spending score of Thomas High School after replacing the ninth graders score.
  
  ![spending_c](https://user-images.githubusercontent.com/95719819/151433548-1038ea0d-e5eb-4e9d-8ac2-99c5b8700b3c.PNG)
  
  Summary of scores by school spending after fomatting.

  ![spending_summary](https://user-images.githubusercontent.com/95719819/151433861-71eb58ec-2977-48d8-8b22-5733404cb4f8.PNG)
  
  - **Scores by school size after replacing math and reading scores for ninth garders**

  Scores by school size of Thomas High School before replacing the ninth graders score.
  
  ![size1](https://user-images.githubusercontent.com/95719819/151433271-329791c4-8e7d-4b2b-bfb8-8f8c16d34bf6.PNG)

  Scores by school size of Thomas High School after replacing the ninth graders score.
  
  ![size_c](https://user-images.githubusercontent.com/95719819/151433306-756b429b-7d14-483b-a7c3-1ca47dbc8f82.PNG)
  
  Summary of scores by school size after fomatting.
  
  ![school size](https://user-images.githubusercontent.com/95719819/151266036-246fa76b-3048-40fd-b6d8-058a46e8a6df.PNG)

  - **Scores by school type after replacing math and reading scores for ninth garders**

  Scores by school type before replacing the ninth graders score in Thomas High School.
  
  ![type1](https://user-images.githubusercontent.com/95719819/151433397-0fe27a83-1cd6-4861-a321-ef34b1760dc7.PNG)
  
  Scores by school type after replacing the ninth graders score in Thomas High School.
  
  ![type_c](https://user-images.githubusercontent.com/95719819/151433429-12dd63b2-61e0-47c6-87cc-3b2a74cd212d.PNG)

  Summary of scores by school type after fomatting the values.

  ![school type](https://user-images.githubusercontent.com/95719819/151266092-8faa82fc-1b73-4d1a-ba96-fcb37da41fc7.PNG)

## Summary
  
  With the above results we summarize our school_district analysis as
  
  - The district summary of the school data showed a very small change in the average scores and the pass percentage.

      



