# Syllabus-MG1
# Introduction to multigrid methods with applications to elliptic and hyperbolic problems
* **Course:** [CMSE801, MSU](https://cmse.msu.edu/ "class home page?????")
* **Instructor:** Mark Adams, [adams@msu.edu](adams@msu.edu "Instructor")
* **Need help?**
    * Look through and create [issues](https://github.com/multigrid-courses/Syllabus-MG1/issues)
    * Office Hours: 
   * [Email](adams@msu.edu) for 1-on-1 help, or to set up a time to meet

## Course Description

This is a graduate level coarse on Multigrid methods and is intended for a wide audience in the
computational sciences.  Some analysis is presented but advanced multigrid
theory, which is thoroughly covered by
[Hackbusch (1985)](https://books.google.com/books/about/Multi_grid_methods_and_applications.html?id=Vf8_AQAAIAAJ),
is not presented. A basic knowledge of analysis, partial differential equations, and
numerical methods is assumed, as well as some experience with
programming. We use Matlab from programming assignments and
Git, hosted at [GitHub](https://github.com), for code and document management.
This coarse introduces some ideas in modern software engineering such
as distributed repositories and collaboration.

##  Overview of Multigrid Course Series 

1. **MG1**: Introduction to multigrid methods with applications to elliptic and
   hyperbolic problems (this course)
1. **MG2**: Algebraic Multigrid with application to elasticity
1. **MG3**: Contemporary Multigrid: hybrid structured/unstructured adaptive mesh refinement, hyperbolic
  problems with geometric multigrid, on emerging architectures,
  advance scientific software engineering in the Portable Extensible
  Toolkit for Scientific Computing (PETSc) with applications to
  magnetohydrodynamics and computational fluid dynamics.

## Prerequisites for MG1

* A numerical analysis course (MSE XXX or equivalent)
* A laptop in class for exercises, etc.

These won't be enforced by the instructor, but you will be pretty lost
without some numerical analysis background, and not having a laptop
will encumber some hands-on class work.

* Some familiarity with
  [Git and GitHub](https://help.github.com/articles/good-resources-for-learning-git-and-github) is
  suggested.
* Students should create a personal account on
[GitHub](https://github.com/join) before the first class

## Course Overview

We will cover basic iterative methods, Local Fourier Analysis (LFA),
and two grid analysis. We go over basic smoother methods and intergrid
transfer operators and analysis their potential efficacy on model
elliptic and hyperbolic problems. We will consider operator dependent
intergrid transfer operators and applications to problems in
computational fluid dynamics.

Students will develop a multigrid solver in Matlab for programming
projects and Git, hosted at [GitHub](https://github.com), for code and
document management.

The course will be co-instructed, via advanced teleconferencing
facilities, with courses at Rice University and KAUST.

## Course Material

* [*An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf)
by Wesseling, is used as the main text
	- May ignore discussion on meshing, parallel programing,
      "structure diagrams", and skip ILU and complexity analysis
* [*Multigrid*](https://books.google.com/books?id=-og1wD-Nx_wC)
Trottenberg, Oosterlee, and Schüller, is an excellent book and is
recommended as a reference
	- My multigrid bible
* [*A Multigrid Tutorial*](https://books.google.com/books/about/A_Multigrid_Tutorial.html?id=oSTGBm64o1AC)  by Briggs, Henson, and McCormick, is a good general multigrid tutorial
	- Go U.S.A.

### Workflow

All code and documents will be managed using Git and hosted on [GitHub](https://github.com).
Here are the overall steps to turning in a homework assignment:

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
git push -u origin name/hw1
```
1. [Create a pull request](https://help.github.com/articles/creating-a-pull-request/) on the original repository. All assignments are due at the start of the following class, unless otherwise specified.
1. You can continue to push fixes and improvements until the close date (listed in Classes) – just add a comment in the pull request to let us know it's been updated.

Feedback will be given in the pull request, so please respond with your thoughts and questions!  You are welcome to open the pull request as the work is still in-progress if you are stuck and want to ask a question – just mention `@adams` with the question to make sure I know to look at it sooner.

### Requirements

* Any borrowed code must be properly [annotated](http://documentup.com/advanced-js/syllabus#statements-on-plagiarism/instructor).
* Bonus points for Creativity (as long as requirements are fulfilled)

## Course Outline

### Class 1

1. Introduction to multigrid history, history of programming paradigms
in scientific computing, applications of multigrid and outline of
three course multigrid series, for which this is the first.
1. Setup Git workflow work on student's laptops, add a line in the
  [class roster](https://github.com/multigrid-courses/Syllabus-MG1/roster.md)
  and submit a pull request.
1. Multigrid framework: local and global processing [Y5:32]

[class roster in Markdown file: name, year, major, do you have an application in mind?, ]

#### Homework

* [Wesselings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 1 & 2.1 - 2.4
* Exercise 2.2.1 in Wesseling (HW1)
* Exercise 0 & 1 from Yavneh

### Class 2

1. Analysis of simple iterative method and multilevel application [Y33-47,Y48-54]
1. The model problem, cyclic reduction, [Y48-53]

### Class 3

1. 2D model problem [Y60-90]

#### Homework

* [Wesselings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 3.1-3.5
* Exercise 2 from Yavneh (HW2)

### Class 4

1. 2D model problem (continued) [Y60-90]
1. First multilevel algorithm

### Class 5

1. 1D Model problem revisited - 1D analysis [Y91-104]
1. Multigrid debugging

#### Homework

* [Wesselings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf)
  Ch. 4 (basic iterative methods, skim ILU)
* Exercise 3 from Yavneh (HW3)

### Class 6

1. IR/ICG Analysis [Y102-115] 

### Class 7

1. Local Fourier Analysis [Y116-~130] 

#### Homework

* [Wesselings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 5
* Exercise 4 from Yavneh (HW4)

### Class 8

1. Local Fourier Analysis (continued) [Y~130-151]  

### Class 9

1. H-Ellipticity [Y152-163] 

#### Homework

* [Wesselings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf)  Ch. 3.6, 3.6, 6 (coarse grid approximations and two grid analysis)
* Exercise 5 from Yavneh (HW5)

### Class 10

1. Finish up LFA and H-Ellipticity

### Class 11

1. Hyperbolic and asymmetric problems [Y164-191]

#### Homework

* Yavneh, "Coarse-Grid Correction of Nonelliptic Problems", SISC 19 (5), 1682-1699 (1998)
* [Wesselings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf)
  Ch. 7 (smoothing analysis)
* Exercise 6 from Yavneh (HW6)

### Class 12

1. Skills used for smoothing parameters

### Class 13

1. Fourier analysis of red-black relaxation [Y192-206]


#### Homework

* Exercise 8 from Yavneh  (HW7)

### Class 14

1. Intergrid transfer and non-ellipticity [Y207-240]

### Class 15

1.  Intergrid transfer and non-ellipticity (continued)  [Y207-240]

#### Homework

* [Wesselings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf)  Ch. 8 (multigrid algorithms)
* Exercise 9 from Yavneh (HW8)
  
### Class 16

1. Indefinite operators [Y241-244]
1. Full multigrid [Y245-249]
1. Nonlinear multi grid and tau correction [Y250-258]

### Class 17

1. Double discretization [Y259-272]
1. Systems 

#### Homework

* Exercise 10 from Yavneh (HW9)

### Class 18

1. Emerging architectures, parallel programming models and algorithms

### Class 19

1. Emerging architectures, parallel programming models and algorithms (cont)

#### Homework

* [Wesselings's *An Introduction to Multigrid Methods*](http://docs.mak.ac.ug/sites/default/files/An%20Introduction%20to%20Multigrid%20Methods,%20by%20Pieter%20Wesseling.pdf) Ch. 9 (CFD)
* Exercise Wesseling ?????

### Class 20

1. Multigrid methods for computational fluid dynamics

### Class 21

1. Multigrid methods for computational fluid dynamics

#### Homework


### Class 22

1. Multigrid methods for computational fluid dynamics

### Class 23

1. Multigrid methods for computational fluid dynamics

#### Homework

* 

### Class 24

1. Multigrid methods for computational fluid dynamics

### Class 25

1. Multigrid methods for magnetohydrodynamics

#### Homework

*

### Class 26

1. Modern mesh generation for fast multigrid solvers - hybrid
   structured/unstructured forest of octrees.

### Class 27

1. Modern mesh generation for fast multigrid solvers - hybrid
   structured/unstructured forest of octrees.

## [Statements on Plagiarism](https://www.msu.edu/~ombud/academic-integrity/plagiarism-policy.html)

Reuse and building upon ideas or code are major parts of modern software development.  As a professional programmer you will never write anything from scratch.  This class is structured such that all solutions are public.  You are encouraged to learn from the work of your peers.  I won't hunt down people who are simply copying-and-pasting solutions, because without challenging themselves, they  are simply wasting their time and money taking this class.

Please respect the terms of use and/or license of any code you find, and if you reimplement or duplicate an algorithm or code from elsewhere, credit the original source with an inline comment.

## License

