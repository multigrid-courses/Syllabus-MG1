# Syllabus-MG1
# Introduction to multigrid methods with applications to elliptic and hyperbolic problems
* **Course:** [CMSE801, MSU](https://cmse.msu.edu/)
* **Instructor:** Mark Adams, [adams@msu.edu](adams@msu.edu)
* **Need help?**
    * Look through and create [issues](https://github.com/multigrid-courses/Syllabus-MG1/issues)
    * Office Hours: 
   * [Email](adams@msu.edu) for 1-on-1 help, or to set up a time to meet

## Course Description

Introduction to classic geometric multigrid methods,
theory and practice, for elliptic and hyperbolic problems.  Algebraic
multigrid methods and methods for emerging architectures
will be covered in subsequent courses.

This is a graduate level coarse intended for a wide audience in the
computational sciences.  Some analysis is presented but advanced multigrid
theory, which is thoroughly covered by Hackbusch (1985), is not
presented; we will use the Wesseling (1992) book *An introduction to
multigrid methods*;  Trottenberg et al, *Multigrid* is an excellent
book and is recommended as a reference.
A basic knowlege of analysis, partial differential equations, and
numerical methods is assumed, as well as Matlab programming.

##  Overview of Multigrid Course Series 

1. Introduction to multigrid methods with applications to elliptic and
   hyperbolic problems (this course)
1. MG2: Algebraic Multigrid with application to elasticity
1. MG3: Contemporary Multigrid: hybrid structured/unstructured adaptive mesh refinement, hyperbolic
  problems with geometric multigrid, on emerging architectures,
  advance scientific software engineering in the Portable Extensible
  Toolkit for Scientific Computing (PETSc) with applications to
  magnetohydrodynamics and computational fluid dynamics.

## Prerequisites

* A numerical analysis course (MSE XXX or equivalent)
* A laptop in class for exercises and debugging Git workflow, etc.

These won't be enforced by the instructor, but you will be pretty lost
without some numerical analysis background, and not having a laptop
will encumber some hands-on class work.

## Course Overview

We will cover basic iterative methods, Local Fourier Analysis (LFA),
and two grid analysis. We go over basic smoother methods and intergrid
transfer operators and analysis their potential efficacy on model
elliptic and hyperbolic problems. We will consider operator dependent
intergrid transfer operators and applications to problems in
computational fluid dynamics.

Students will develop a simple multigrid solver in Matlab.

The course will be co-instructed, via advanced teleconferencing
facilites, with courses at Rice University and KAUST.

## Homework/Projects

Homework assignment will be given weekly as well as programming
assignments.
Git, hosted on github.com, will be used for all documents

### Workflow

All documents will be communicated using Git and hosted on github.com.
Here are the overall steps:

1. Fork the repository for the exercise or project (found under [github.com/multigrid-courses](https://github.com/multigrid-courses)).
1. Clone the repository to your computer:
```
git clone git@github.com:multigrid-courses/MG1-HW1
```
1. Modify the files to complete your solution.
1. Make sure all of your code is committed:
```
git commit -am"all done"
```
1. Push to GitHub to a branch user/assignment:
```
git push -u origin adams/hw1
```
1. [Create a pull request](https://help.github.com/articles/creating-a-pull-request/) on the original repository. All assignments are due at the start of the following class, unless otherwise specified.
1. You can continue to push fixes and improvements until the close date (listed in Classes) – just add a comment in the pull request to let us know it's been updated.

Feedback will be given in the pull request, so please respond with your thoughts and questions!  You are welcome to open the pull request as the work is still in-progress if you are stuck and want to ask a question – just mention `@adams` with the question to make sure I know to look at it sooner.

### Requirements

These apply to real life, as well.

* Any borrowed code must be properly [annotated](http://documentup.com/advanced-js/syllabus#statements-on-plagiarism/instructor).
* Bonus points for:
    * Automated tests
    * Creativity (as long as requirements are fulfilled)

## Course Outline

### Class 1

1. Introduction to multigrid history, history of programming paradigms
in scientific computing, applications of multigrid and outline of
three course multigrid series, for which this is the first.
1. Setup Git workflow work on student's laptops
1. Multigrid framework: local and global processing [Y5:32]

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 1 & 2.1 & 2.2
* Exercise 2.2.1 in Wesseling (HW1)

### Class 2

1. Analysis of simple iterative method and multilevel application [Y33-46,Y60-87]

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 0 from Yavneh (HW2)

### Class 3

1. The model problem, cyclic reduction, [Y47-53]

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 1 from Yavneh (HW3)


### Class 4

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling


### Class 5

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling


### Class 6

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling


### Class 7

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling


### Class 8

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling


### Class 9

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling


### Class 10

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling


### Class 11

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling


### Class 12

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling


### Class 13

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling


### Class 14

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling


### Class 15

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling


### Class 16

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling


### Class 17

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling



### Class 18

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling



### Class 19

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling



### Class 20

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling



### Class 21

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling



### Class 22

1. 

#### Homework

* [Wesslings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 
* Exercise 2.2.1 in Wesseling


### Class 23

1. Multigrid methods for computational fluid dynamics

#### Homework

* 

### Class 24

1. Multigrid methods for computational fluid dynamics

#### Homework

* 
### Class 25

1.  Multigrid methods for magnetohydrodynamics

#### Homework

*

### Class 26

1. Modern mesh generation for fast multigrid solvers - hybrid
   structured/unstructured forest of octrees.

#### Homework


### Class 27

1. Modern mesh generation for fast multigrid solvers - hybrid
   structured/unstructured forest of octrees.

#### Homework


## [Statements on Plagiarism](https://www.msu.edu/~ombud/academic-integrity/plagiarism-policy.html)

Reuse and building upon ideas or code are major parts of modern software development.  As a professional programmer you will never write anything from scratch.  This class is structured such that all solutions are public.  You are encouraged to learn from the work of your peers.  I won't hunt down people who are simply copying-and-pasting solutions, because without challenging themselves, they  are simply wasting their time and money taking this class.

Please respect the terms of use and/or license of any code you find, and if you reimplement or duplicate an algorithm or code from elsewhere, credit the original source with an inline comment.

## License

