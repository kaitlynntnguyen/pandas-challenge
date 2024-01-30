# Pandas-Challenge
1. First, I loaded the data from a csv file containing all school data, `schools_complete.csv`, and a csv file containing all student data, `students_complete.csv`. I used `merge()` to store the school and student data in one dataframe.

2. I created a district summary by using `count()` to obtain the number of schools in the dataset and to obtain the total number of students in the dataset. I used `sum()` to calculate the total budget of the district. I used `mean()` to calculate the average math and reading scores of the district, calculated the percentage of students passing math, the percentage of students passing reading, and the percentage of students passing both. I stored this data in a dataframe.

3. I created a list of the schools and what type of school they are, district or charter, by selecting only the `school_name` and `type` columns from the dataset and using `groupby()` to show each school only once in the list.

4. I used `value_counts()` to obtain the number of students in each school. I obtained the budget of each school and divided it by the number of students to obtain the budget per student. I also obtained the average math score and average reading score per school. I obtained the percentage of students passing math, the percentage passing reading, and the percentage passing both for each school. I used this data to create a school summary.
Average reading score

5. I acquired the names of the highest performing school based on the percentage of students passing both math and reading using `sort_values()` on the `% Overall Passing column`. The top 5 performing schools were:
      - Cabrera High School
      - Thomas High School
      - Griffin High School
      - Wilson High School
      - Pena High School.
  -All of these schools are charter schools.
  -Three of the top schools have a total number of students between 1000 and 2000, one of the            schools has a total number of students below 1000, and one of the schools has a total number of       students above 2000.
  -Two of the schools have a per students budget below $585, two of the schools have a per student     budget between $585 and $630, one school has a per student budget between $630 and $645.

6. I acquired the names of the lowest performing school based on the percentage of students passing both math and reading, I used sort_values() on the % Overall Passing column. The bottom 5 performing schools were:
      - Rodriguez High School
      - Figueroa High School
      - Huang High School
      - Hernandez High School
      - Johnson High School.
  - All of these schools are district schools
  - All of the schools have a total number of students between 2000 and 5000
  - Two of the schools have a per students budget between $630 and $645, three of the schools have a     per student budget between $645 and $680.
    
7. I calculated the average math scores and average reading scores of each school by grade.
  
8. I divided school spending per student into four categories and displayed the average math score, average reading score, % passing math, % passing reading, and % overall passing.
The categories are:
    - <$585: the averages and percentage of passing students are the highest in this group across all categories.
    - $585-630: this group is the second best performing across all categories.
    - $630-645: this group is the third best performing across all categories. -$645-680: the averages and percentage of passing students are the lowest in this group across all categories.
  
9. I divided schools by number of students into three categories and displayed the average math score, average reading score, % passing math, % passing reading, and % overall passing.
The categories are:
    - Small (<1000): this group has the highest average math score, and the highest average reading score.
    - Medium (1000-2000): this group has the highest % passing math, % passing reading, and % overall passing.
    - Large (2000-5000): this group is the worst performing across all categories.
There is not much difference between the averages and % passing of small and medium schools.

10. I divided the schools by school type and displayed the average math score, average reading score, % passing math, % passing reading, and % overall passing.
    - Charter: charter schools perform better across all categories.
    - District: district schools perform worse across all categories.
