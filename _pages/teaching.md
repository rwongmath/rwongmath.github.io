---
permalink: /teaching/
title: "Teaching"

layout: single

toc: true
toc_label: "Content"
toc_icon: "chalkboard-teacher"

---


{% assign statement = site.static_files | where: "basename", "Richard_Wong_Teaching_Statement" | first %}

> "It seems to me that the poet has only to perceive that which others do not perceive, to look deeper than others look. And the mathematician must do the same thing." 

<cite>--- [Sofya Kovalevskaya](https://en.wikipedia.org/wiki/Sofya_Kovalevskaya)</cite>
{: .small} 

Teaching and communicating mathematics is an important part of my mathematical identity, and I value the impact that I have as an educator. It is for this reason that I am committed to *inclusive and equitable teaching* that *affirms and empowers* students.

My **[Teaching Statement](/assets/Richard_Wong_Teaching_Statement.pdf)** can be found here (last updated {{ statement.modified_time | date: '%B %Y' }}).

My full **Teaching Portfolio** (which contains student evaluations, teaching materials, and sample syllabi) is available upon request. Here are some [sample teaching materials](/teaching/materials).  

<!--end_excerpt-->

<hr>

# Teaching Philosophy:

I strongly believe that EVERYONE is capable of success in mathematics, and I want my students to discover that mathematics can be inspiring, affirming, and even empowering.  There are two key principles that drive my teaching philosophy:

In my classes, I use **active** and **inquiry-based learning techniques**, and I teach my students how to use questioning as a tool to clarify concepts, to stimulate new ideas, and most importantly, to communicate mathematics.

Moreover, I design my courses with an emphasis on **student collaboration**, and I strive to create **positive and inclusive learning environments** where all students feel welcome to ask questions, work with each other, and to voice their ideas. 

<hr>

# Courses Taught:

## UCLA

<ul>
{% for course in site.courses_taught %}
{% if course.school == "UCLA" %}	
  <li>
  <a href="{{ course.url }}">{{ course.title }}</a>
  </li>
{% endif %}
{% endfor %}
</ul>


## UT Austin

<ul>
{% for course in site.courses_taught %}
{% if course.school == "Texas" %}	
  <li>
  <a href="{{ course.url }}">{{ course.title }}</a>
  </li>
{% endif %}
{% endfor %}
</ul>

## Other Experience

* From Summer 2017-2021, I have either taught or co-taught [Summer Minicourses](https://web.ma.utexas.edu/SMC/) on homological algebra and/or spectral sequences. 
	* Each minicourse is a week of lectures and problem sessions designed to teach graduate and advanced undergraduate students tools, methods, or ideas in research-level mathematics.
* I have mentored 9 undergraduate reading projects on various topics in algebra, topology, and homotopy theory through the [UT Austin Directed Reading Program](https://web.ma.utexas.edu/users/drp/) (DRP).

## TA Experience

* TA for [UGS 303: From Numbers to Chaos](/teaching/UGS_303) at UT Austin.
* TA for M 408M: Multivariable Calculus at UT Austin.
* SI leader for M 408K: Differential Calculus at UT Austin.
* TA for the [Young Scholars Program in Discrete Mathematics](http://dimacs.rutgers.edu/archive/ysp/).
* Mathematics Peer Mentor for 152H, 192H, 251H, 291H, and 292H at Rutgers University.

<hr>

# Seminars, Workshops, and Awards:

Throughout my career, I have participated in various seminars, workshops, and programs to continue to learn about teaching and education.

## Awards

* **Liggett Instructor Teaching Award**, UCLA Spring 2023
* **SSD Appreciation Award** (“Clock Award”), UT Austin Spring 2021
* **FIC Graduate Student Teaching Award**, UT Austin Spring 2020
{: reversed="reversed"}

## Seminar Talks

{% include /list_teachingseminar.md %}

## Workshops

0. [CEILS Summer Institute: Foundations of Equitable Course Design](https://ceils.ucla.edu/learning-communities-trainings/summer-institute-on-scientific-teaching/), Summer 2022
0. [CEILS Annual Faculty Workshop on Best Equitable Practices In Teaching](https://ceils.ucla.edu/ceils-annual-faculty-workshop21/), Summer 2021
0. [New Faculty Teaching Engagement (NFTE) workshop](https://teaching.ucla.edu/faculty-programs/new-faculty-teaching-engagement/), Summer 2021
0. [Concentration in Communicating Science](https://cns.utexas.edu/info-graduate-students-postdocs/electives-concentrations), Spring 2019
0. [Teaching Preparation Certificate](https://ctl.utexas.edu/programs-initiatives/graduate-student-development), Spring 2018
0. [Inclusive Classrooms Leadership Certificate](https://equity.utexas.edu/inclusive-classrooms-seminar/), Fall 2017
0. [Supplemental Instruction](https://ugs.utexas.edu/slc/support/si) Training, Fall 2017
0. M 398T: Supervised Teaching in Mathematics, Fall 2015
{: reversed="reversed"}

