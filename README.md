
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


# [MSGAI] Modeling and Scaling Generative AI Systems <!-- omit in toc -->

This repository contains the materials of the **MSc Modeling and Scaling for Generative AI systems** course running in fall 2024 at UNINE.


##  1. <a name='Importantlinks'></a>Important links

- [Project description](project.md)
- [Labs and assignments](lab.md)


##  2. <a name='Coursedescription'></a>Course description


Todays machine learning systems become the backbone technology for our daily life.  Generative AI (GAI) systems, such as language models and diffusion models, are widely used to generate texts, images, videos, and tables. It is challenging to design and run the inference of GAI system that guarantee users’ performance requirements, e.g., latency constraint, in a resource efficient way. Various quantitative methods are applied to capture such complex system dynamics and predict metrics of interests, from the designing phase of the systems to the runtime performance, e.g., job response times and system anomaly.  To optimize the performance of GAI  systems, a deep understanding on those methods and their applications on the system design are essential. 
<!-- Having practical hand-on experience on designing experiments, deriving models, and validating results with benchmark systems will prepare students to tackle challenges of real systems. -->

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
-  [Jiyue Huang](mailto:J.Huang-4@tudelft.nl) (TUD Postdoc)


Lydia is the responsible instructors of this course and can be reached at **lydiaychen@ieee.org**.



##  4. <a name='Learningobjectives'></a>Learning objectives
- LO1. Understanding the training and sampling of generative models, namely diffusion and language models 
- LO2. Design full/fractional factorial experiments for multi-variate regression analysis, e.g., finding critical parameters for GAI systems
- LO3 Apply queueing theory to analyse and predict the run-time performance of applications, e.g., the average response times of on-line GAI sampling service
- LO4. Develop resource management policies for GAI systems and validate them on real computing systems


## 5. <a name='dart:Gradingpolicy'></a>:dart: Grading policy

This course has no final exam, instead the grade is largely determined through three components: 

1. Homework (30%): 3 individual homework due in week 4, 8, 12. Each homework accounts 10  of the grade and cover 4 weeks material. All homework will be released at the begining of the semester.


2. Group project (70%): group project report (60%) and presentation (10%). There will be topics of modeling response times, configuring, dependability, scheduling design. There will be an initial proposal in week 6, interim discussion with each team in week 10. The final report will be due in week 13, and 20 minutes presentation in week 9 as well.


**All assessment items (homework, and projects reports) have to be submitted via ILIAS.**


###  5.1. <a name='Homework'></a>Homework
- Homework 1: due in week 4 
- Homework 2: due in week 8
- Homework 3: due in week 12

Students are given additional 48 hours grace period for late submission and will not receive any grade penalty. However, submissions after 48 hours grace period will not be considered and students will loose 25 points of their final grade. 


###  5.2. <a name='Groupprojects'></a>Group projects
<!-- 7 predefined project topics: evaluating the systems of 
-->
There are different aspects of performance  on modeling and optimizing the executions of deep neural network jobs. In this project, you will play with benchmarks that emulate the training jobs of deep neural networks on top of Spark platform - one of the most popular platform. You can build a model to predict the performance such jobs, to optimize their response times through resource allocations and scheduling, and to test the dependability of such a cluster against malicious attacks. You will do this project in a group with 1-2 other peers.

- Group size: 1-2 students
- Schedule: 
  - Initial proposal: week 6
  - Interim meeting: week 10
  - Report due: week 13
  -  Presentation/interview: week 13 



At the end of each project phase we will conduct a short interview (20 minutes per group) about the group project and its connection to the course content. Based on the project report and the interview, each member of the group receives a grade. 





##  6. <a name='Detailedschedule'></a>Detailed schedule


**Week**|**Lecture Topic**|**Lab Topic**|**Assigment Due**
:-----|:-----|:-----|:-----
Week 1 (Sep 23) | Introduction on Generative AI| Setup & Intro
Week 2 (Sep 30) | Diffusion Model | DM
Week 3 (Oct 7) | Diffusion Model II | Fast DM inference| 
Week 4 (Oct 14) | Transformers | HW1 | HW1
Week 5 (Oct 21) | Language Models I | Transformers 
Week 6 (Oct 28) | Language Model II |Prompt engineering|Project proposal
Week 7 (Nov 4) | DoE I | Q/A on H2 |
Week 8 (Nov 11) | DoE II  | No Lab | HW2
Week 9 (Nov 18) | DTMC | Job generator | Project midterm
Week 10 (Nov 25) | CTM| No Lab | 
Week 11 (Dec 2) | Queueing (Flip Class)  |  Q/A on HW3
Week 12 (Dec 9) | Extra session on the project |  | HW3
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
- [Design and Analysis of Experiments](http://faculty.business.utsa.edu/manderso/STA4723/readings/Douglas-C.-Montgomery-Design-and-Analysis-of-Experiments-Wiley-2012.pdf) by Douglas Montgomery
- [Dive into Deep Learning](https://www.d2l.ai/) by Alex Smola et. al.
- [Pattern Recognition and Machine Learning]() by Christopher Bishop 





