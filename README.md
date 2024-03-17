
:warning: **I am still developing the course content. The content will be only be finalized by the end of the first week of the semester.**

<!-- vscode-markdown-toc -->
* 1. [Important links](#Importantlinks)
* 2. [Course description](#Coursedescription)
* 3. [Course team](#Courseteam)
* 4. [Learning objectives](#Learningobjectives)
* 5. [:dart: Grading policy](#dart:Gradingpolicy)
	* 5.1. [Homework](#Homework)
	* 5.2. [Group projects](#Groupprojects)
* 6. [Detailed schedule](#Detailedschedule)

	
<!-- vscode-markdown-toc-config
	numbering=true
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc --><!-- vscode-markdown-toc -->


# QPEC <!-- omit in toc -->

This repository contains the materials of the **MSc Modeling and Scaling for Generative AI systems** course running in fall 2024 at UNINE.


##  1. <a name='Importantlinks'></a>Important links

- [Project description](project.md)
- [Labs and assigments](homework.md)


##  2. <a name='Coursedescription'></a>Course description




Todays computing systems become ever complex, due to the rapid development of hardware and software technology.  It is challenging to design and run computing systems that guarantee users’ performance requirements in a resource efficient way. Various quantitative methods are applied to capture such complex system dynamics and predict metrics of interests, from the designing phase of the systems to the runtime performance, e.g., job response times and system anomaly.  To optimize the performance of computing systems, a deep understanding on those methods and their applications on the system design are essential. Having practical hand-on experience on designing experiments, deriving models, and validating results with benchmark systems will prepare students to tackle challenges of real systems. 

Course topics include
- Generative adversarial networks
- Diffusion models
- Large langague models
- Design of experiments and statistical tests 
- Operational laws and queueing methods for modeling GAI systems
- Scheduling and load balancing for GAI systems







##  3. <a name='Courseteam'></a>Course team

This course will be mainly taught by [Prof. Lydia Y Chen](https://lydiaychen.github.io/)  The course team is composed of a number of PhDs  who support the course through guest lectures and project supervision and a TA who focuses on the grading of homework. 


-  [Jeroen Galjaard](mailto:J.M.Galjaard@tudelft.nl) (TUD PhD student)


Lydia is the responsible instructors of this course and can be reached at **lydiaychen@ieee.org**.



##  4. <a name='Learningobjectives'></a>Learning objectives
- LO1. Design full/fractional factorial experiments for multi-variate regression analysis, e.g., finding critical parameters for Generative AI clusters.
- LO2. Apply queueing theory to analyse and predict the run-time performance of applications, e.g., the average response times of on-line ML training service.
- LO3. Apply machine learning models to analyse and predict the system dependability, e.g, root cause analysis for machine failure.
- LO4. Conduct experiments to profile applications and extract their workload parameters on real systems, e.g., deep learning clusters
- LO5. Develop resource management policies and validate them on real computing systems, e.g., deep learning clusters


## 5. <a name='dart:Gradingpolicy'></a>:dart: Grading policy

This course has no final exam, instead the grade is largely determined through three components: 

1. Homework (30%): 3 individual homework due in week 4, 8, 11. Each homework accounts 10  of the grade and cover 3 weeks material. All homework will be released at the begining of the semester.


2. Group project (70%): group project report (60%) and presentation (10%). There will be topics of modeling response times, configuring, dependability, scheduling design. There will be an initial proposal in week 5, interim discussion with each team in week 9. The final report will be due in week 13, and 20 minutes presentation in week 9 as well.


**All assessment items (homework, and projects reports) have to be submitted via ILIAS.**


###  5.1. <a name='Homework'></a>Homework
- Homework 1: due in week 4 
- Homework 2: due in week 8
- Homework 3: due in week 112

Students are given additional 48 hours grace period for late submission and will not receive any grade penalty. However, submissions after 48 hours grace period will not be considered and students will loose 25 points of their final grade. 


###  5.2. <a name='Groupprojects'></a>Group projects
<!-- 7 predefined project topics: evaluating the systems of 
-->
There are different aspects of performance  on modeling and optimizing the executions of deep neural network jobs. In this project, you will play with benchmarks that emulate the training jobs of deep neural networks on top of Spark platform - one of the most popular platform. You can build a model to predict the performance such jobs, to optimize their response times through resource allocations and scheduling, and to test the dependability of such a cluster against malicious attacks. You will do this project in a group with 1-2 other peers.

- Group size: 1-2 students
- Schedule: initial proposal (week 5), interim meeting (week 9), report due (week 13), and presentation/interview (week 13). 

[UPDATE] We change the requirement. For the final project, you just need to submit ppt slides, which summarize the results. If you submit a report, you will be getting bosnus point.

At the end of each project phase we will conduct a short interview (20 minutes per group) about the group project and its connection to the course content. Based on the project report and the interview, each member of the group receives a grade. 





##  6. <a name='Detailedschedule'></a>Detailed schedule


**Week**|**Lecture Topic**|**Lab Topic**|**Assigment Due**
:-----|:-----|:-----|:-----
Week 1 (Sep 23) | Introduction on Generative AI| Setup & Intro
Week 2 (Sep 30) | Generative Adversarial Networks | GANs
Week 3 (Oct 7) | Diffusion Models | DM
Week 4 (Oct 14) | Transformers | HW1 | HW1
Week 5 (Oct 21) | Large Langauge Model I | Transformer | Project proposal
Week 6 (Oct 28) | Largue Lanague Model II/Project | Prompt Engineering
Week 7 (Nov 4) | DoE I | Performance benchmarking |
Week 8 (Nov 11) | DoE II  | HW2 | HW2
Week 9 (Nov 18) | Operational Law |  | Project midterm
Week 10 (Nov 25) | DTMC| DTMC
Week 11 (Dec 2) | Queueing theorey | CTMC
Week 12 (Dec 9) | Scheduling | HW3 | HW3
Week 13 (Dec 16) | Project presentation | No Lab



##  7. <a name='Relevantreferences'></a>Relevant references 

### 7.1 <a name='Onlinelecturenotes'></a>Online lecture notes

 - [Design of Experiments](https://newonlinecourses.science.psu.edu/stat503/node/5/), Penn State University
 - [Computer System Performance Evaluation](http://www.cse.cuhk.edu.hk/~cslui/csc5420.html) , John C.S. Lui at CUHK
- [Data Mining](http://personal.psu.edu/jol2/course/stat557/), Jia Li at Penn State University
-  [Introduction to Machine learning](http://www.cs.cmu.edu/~epxing/Class/10701/), Eric Xing at Carnagie Mellon University



###  7.2. <a name='Booksonperformancemodeling'></a>Books on performance modeling
- Introduction to Probability Models by S. M. Ross, 
- Quantitative System Performance by E. Lazowska, J. Zahorjan, S. Graham, and K. Sevcik.
- Capacity Planning and Performance Modeling by D. Menasce, V. Almeida, and L. Dowdy 


###  7.3. <a name='Booksonstatisticalexperimentsandlearning'></a>Books on statistical experiments and learning
- [Design and Analysis of Experiments] (http://faculty.business.utsa.edu/manderso/STA4723/readings/Douglas-C.-Montgomery-Design-and-Analysis-of-Experiments-Wiley-2012.pdf) by Douglas Montgomery
- [Dive into Deep Learning](https://www.d2l.ai/) by Alex Smola et. al.
- [Pattern Recognition and Machine Learning]() by Christopher Bishop 





