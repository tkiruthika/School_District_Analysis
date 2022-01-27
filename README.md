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
  
## Challenge
  
  It was said that there is a academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appears to have been altered. So, we are asked to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. After replacing we need to repeat the school district analysis.

## Results

  **- District Summary**

  ![district_summary2](https://user-images.githubusercontent.com/95719819/151267048-26fdcbe0-0a09-48c1-b5ce-c8c199e3df6e.png)
  
  **- School Summary**
  
  ![school summary 2](https://user-images.githubusercontent.com/95719819/151247387-29be27c0-f57d-4f2b-8ccc-9666c1216fc0.PNG)
  
  **- Thomas High School’s performance relative to the other schools after replacing math and reading scores for ninth garders**
  
  ![school summary](https://user-images.githubusercontent.com/95719819/151248352-c5c3d353-9628-470d-bdba-29b141122bb8.PNG)
  
  **- Top 5 performing schools, based on the overall passing rate**

  ![top 5](https://user-images.githubusercontent.com/95719819/151265626-2bf958d3-1ea9-4b86-bba6-932f1eeb36f8.png)
 
  **- Bottom 5 performing schools, based on the overall passing rate**
 
  ![bottom5](https://user-images.githubusercontent.com/95719819/151265803-4f8286ac-47a1-49f9-8cae-1473f40b31a5.PNG)
  
  **- Math and Reading scores by grade after replacing math and reading scores for ninth garders**
  
  ![math scores](https://user-images.githubusercontent.com/95719819/151265959-a4903810-23a2-44f8-bc12-1aa3b43f5518.PNG)
  
  ![reading scores](https://user-images.githubusercontent.com/95719819/151265977-5c3b8f6c-0c4c-43fb-8187-086f86eda11c.PNG)

  **- Scores by school spending after replacing math and reading scores for ninth garders**
    
  ![spending summary](https://user-images.githubusercontent.com/95719819/151265992-d4a19ece-c8c3-4ff2-9942-0e1e9034652e.PNG)
  
  **- Scores by school size after replacing math and reading scores for ninth garders**
  
  ![school size](https://user-images.githubusercontent.com/95719819/151266036-246fa76b-3048-40fd-b6d8-058a46e8a6df.PNG)

  **-Scores by school type after replacing math and reading scores for ninth garders**
  
  ![school type](https://user-images.githubusercontent.com/95719819/151266092-8faa82fc-1b73-4d1a-ba96-fcb37da41fc7.PNG)

   
 
## Summary
  

      



