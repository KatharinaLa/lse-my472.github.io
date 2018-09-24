---
papersize: a4
documentclass: scrartcl
classoption: DIV=14
colorlinks: true
---

![LSE](images/lse-logo.jpg)
# MY472 Data for Data Scientists

### Michaelmas Term 2018

### Instructors

* [Pablo Barberá](mailto:P.Barbera@lse.ac.uk), Department of Methodology.  *Office hours*: TBA, COL.7.10 (book via LSE for You)

* [Akitaka Matsuo](mailto:A.Matsuo@lse.ac.uk), Department of Methodology.  *Office hours*: TBA, COL.8.02 (book via LSE for You)

### Course Information

* Lectures on Tuesdays 09:00–11:00 in 32L.LG.03
* Classes on:
    - Thursdays 9:30-11:00 STC.S08
    - Fridays 15:00-16:30 STC.S018	

No lectures or classes will take place during School Reading Week 6.

### Course Description

This course will cover the principles of digital methods for storing and structuring data, 
including data types, relational and non­relational database design, and query languages. 
Students will learn to build, populate, manipulate and query databases based on datasets 
relevant to their fields of interest. The course will also cover workflow management 
for typical data transformation and cleaning projects, frequently the starting point 
and most time­-consuming part of any data science project.  This course uses a 
project-based learning approach towards the study of online publishing and 
group­-based collaboration, essential ingredients of modern data science projects. 
The coverage of data sharing will include key skills in on-line publishing, including 
the elements of web design, the technical elements of web technologies and web programming, 
as well as the use of revision-control and group collaboration tools such as GitHub. 
Each student will build one or more interactive website based on content relevant to 
his/her domain­-related interests, and will use GitHub for accessing and submitting 
course materials and assignments.

### Objectives

In this course, we introduce principles and applications of the electronic 
storage, structuring, manipulation, transformation, extraction, and 
dissemination of data. This includes data types, database design, 
data base implementation, and data analysis through structured queries. 
Through joining operations, we will also cover the challenges of data 
linkage and how to combine datasets from different sources. We begin 
by discussing concepts in fundamental data types, and how data is stored 
and recorded electronically. We will cover database design, especially 
relational databases, using substantive examples across a variety of fields. 
Students are introduced to SQL through MySQL, and programming assignments 
in this unit of the course will be designed to insure that students learn to 
create, populate and query an SQL database. We will introduce NoSQL using 
MongoDB and the JSON data format for comparison. For both types of database, 
students will be encouraged to work with data relevant to their own interests 
as they learn to create, populate and query data. In the final section of the 
data section of the course, we will step through a complete workflow including 
data cleaning and transformation, illustrating many of the practical challenges 
faced at the outset of any data analysis or data science project.

Online publishing and collaboration tools forms the second part of this course, 
along with the tools and technologies that underlie them. Students will develop 
interactive, secure and powerful projects for the World Wide Web using both client
 and server side technologies. Collaboration and the dissemination and submission 
 of course assignments will use GitHub, the popular code repository and version 
 control system. The course begins with an in­depth look at the mark­up languages 
 that form the foundations of building web sites with a study of HTML and CSS. 
 Students next study basic programming in JavaScript, to provide client and 
 server side tools including the customization of web content using Bootstrap 
 and Jekyll to publish web pages, which will provide the basis for a class project.

### Assessment

#### Formative coursework

Students will be expected to produce five weekly, structured problem sets with a 
beginning component to be started in the staff-led lab sessions, to be 
completed by the student outside of class. Answers should be formatted and 
submitted for assessment. 

#### Summative Assignments

Take home exam (50%) and in class assessment (50%).

Student problem sets will be marked and will provide 50% of the mark. 

### Recommended Texts

TBA


### Schedule

#### Week 1, October 2 (PB). [Introduction to data](https://github.com/lse-my472/lectures/blob/master/week01/)

In the first week, we will introduce the basic concepts of the course, including how data is recorded, stored, and shared. Because the course relies fundamentally on GitHub, a collaborative code and data sharing platform, we will introduce the use of git and GitHub, using the lab session to guide students through in setting up an account and subscribing to the course organisation and assignments.

This week will also introduce basic data types, in a language-agnostic manner, from the perspective of machine implementations through to high-level programming languages. We will then focus on how basic data types are implemented in R.

Lecture notes:

- Overview of the course
- Lecture week 1: Introduction to data
- R example: vectors, lists, data frames

Readings:

*Required readings*:
* Wickham, Hadley.  Nd.  _Advanced R_, 2nd ed.  Ch 3, [Names and values](https://adv-r.hadley.nz/names-values.html), Chapter 4, [Vectors](https://adv-r.hadley.nz/vectors-chap.html), and Chapter 5, [Subsetting](https://adv-r.hadley.nz/subsetting.html). (Ch. 2-3 of the print edition),
* [GitHub Guides](https://guides.github.com), especially: "Understanding the GitHub Flow", "Hello World", and "Getting Started with GitHub Pages".
* GitHub.  "[Markdown Syntax](https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf)" (a cheatsheet).

*Further Readings*:
* Lake, P. and Crowther, P. 2013. _Concise guide to databases: A Practical Introduction_.  London: Springer-Verlag.  Chapter 1, [Data, an Organizational Asset](https://books.google.co.uk/books?id=SuK2BAAAQBAJ&pg=PA301&lpg=PA301&dq=Concise+Guide+to+Databases+pdf&source=bl&ots=pEJj8miMrf&sig=3nrRgpk3kF7fXzcWUWpJ_uzpfl0&hl=en&sa=X&ved=0ahUKEwiAkM3JrbHWAhXE7xQKHWseCZAQ6AEISzAH#v=onepage&q=Concise%20Guide%20to%20Databases%20pdf&f=false)
* "[Understanding Big and Little Endian Byte Order](https://betterexplained.com/articles/understanding-big-and-little-endian-byte-order/)".  _Better Explained_ website.
* Nelson, Meghan.  2015.  "[An Intro to Git and GitHub for Beginners (Tutorial).](http://product.hubspot.com/blog/git-and-github-tutorial-for-beginners)"
* Jim McGlone, "[Creating and Hosting a Personal Site on GitHub
A step-by-step beginner's guide to creating a personal website and blog using Jekyll and hosting it for free using GitHub Pages.](http://jmcglone.com/guides/github-pages/)".

*Lab*: **Working with git and GitHub**
* Installing git and setting up an account on GitHub
* How to complete and submit assignments using GitHub Classroom
* Forking and correcting a broken Jupyter notebook
* Cloning a website repository, modifying it, and publishing a personal webpage


#### Week 2, October 9 (PB). [The shape of data](https://github.com/lse-my472/lectures/blob/master/week02/)

This week moves beyond the rectangular format common in statistical datasets, modeled on a spreadsheet, to cover relational structures and the concept of database normalization. We will also cover ways to restructure data from "wide" to "long' format, within strictly rectangular data structures. Additional topics concerning text encoding, date formats, and sparse matrix formats are also covered.

*Readings*:
* Wickham, Hadley and Garett Grolemund.  2017.  _R for Data Science: Import, Tidy, Transform, Visualize, and Model Data_.  Sebastopol, CA: O'Reilly.  [Part II Wrangle](http://r4ds.had.co.nz/wrangle-intro.html), [Tibbles](http://r4ds.had.co.nz/tibbles.html), [Data Import](http://r4ds.had.co.nz/data-import.html), [Tidy Data](http://r4ds.had.co.nz/tidy-data.html) (Ch. 7-9 of the print edition).
* The [**reshape2** package](http://had.co.nz/reshape/) for R.

Lecture notes:

- Lecture week 2: the shape of data
- R example: reshaping data in R

*Lab*: **Reshaping data in R**

*Assignment 1*: **Introduction to data cleaning in R**


#### Week 3, October 16 (AM). [Cloud computing](https://github.com/lse-my472/lectures/blob/master/week03/)


#### Week 4, October 23 (AM). [Basics of HTML and CSS](https://github.com/lse-my472/lectures/blob/master/week04/)


#### Week 5, October 30 (AM). [Using data from the internet](https://github.com/lse-my472/lectures/blob/master/week05/)


#### Week 6, November 6. Reading week. No class.


#### Week 7, November 13 (PB). [Working with APIs](https://github.com/lse-my472/lectures/blob/master/week07/)


#### Week 8, November 20 (PB). [Creating and managing databases](https://github.com/lse-my472/lectures/blob/master/week08/)


#### Week 9, November 27 (AM). [Interacting with online databases](https://github.com/lse-my472/lectures/blob/master/week09/)


#### Week 10, December 4 (PB). [Exploratory data analysis](https://github.com/lse-my472/lectures/blob/master/week10/)


#### Week 11, December 4 (PB). [Parallel computing](https://github.com/lse-my472/lectures/blob/master/week11/)

