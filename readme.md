# Introduction to Scientific, Numerical, and Data Analysis Programming in Python

Python is one of the most widely used and highly valued programming languages
in the world, and is especially widely used in data science, machine learning,
and in other scientific computing applications.  In order to use Python
confidently and competently for these applications, it is necessary to have a
solid foundation in the fundamentals of scientific, numerical, and data
analysis programming Python.  This two day course provides a general
introduction to numerical programming in Python, particularly using numpy, data
processing in Python using Pandas, data analysis in Python using `statsmodels`
and `rpy2`. We will also cover the major data visualization and graphics tools in Python, particularly `matplotlib`, `seaborn`, and `ggplot`.
Finally, we will cover some other major scientific Python tools, such as for
symbolic mathematics and parallel programming and code acceleration.  Note that
in this course, we will not be teaching Python fundamentals and general purpose
programming, but this knowledge will be assumed, and is also provided in a
preceding two-day course.

## Intended Audience

This course is aimed at anyone who is interested in learning the fundamentals
of Python generally and especially for ultimately using Python for data science
and scientific applications.

## Teaching Format

This course will be hands-on and workshop based. Throughout each day, there
will be some brief introductory remarks for each new topic, introducing and
explaining key concepts.

The course will take place online using Zoom. On each day, the live video broadcasts will occur between (UK local time) at:

* 10am-12pm
* 1pm-3pm
* 4pm-6pm

All the sessions will be video recorded, and made available immediately on a private video hosting website. Any materials, such as slides, data sets, etc., will be shared via GitHub.

## Assumed quantitative knowledge

We will assume only a minimal amount of familiarity with some general
statistical and mathematical concepts. These concepts will arise when we
discuss numerical computing, symbolic maths, and statistics and machine
learning. However, expertise and proficiency with these concepts are not
necessary. Anyone who has taken any undergraduate (Bachelor's) level course on
(applied) statistics or mathematics can be assumed to have sufficient
familiarity with these concepts.

## Assumed computer background

We assume familiarity with using Python and knowledge of general purpose
programming in Python.  This topics are covered comprehensively in a preceding
two-day course, which will provide all the prerequisites for this course.


## Equipment and software requirements

Attendees of the course must use a computer with Python (version 3) installed.
All the required software, including Python itself, the development and
programming environment tools, and the Python packages, are free and open
source and are available on Windows, MacOs, and Linux. Instructions on how to
install and configure all the software are provided [here](software.md). We will also provide time during the workshops to ensure that all
software is installed and configured properly.

# Course programme

## Day 1

* Topic 1: *Numerical programming with `numpy`*. Although not part of Python's
  official standard library, the `numpy` package is the part of the de facto
  standard library for any scientific and numerical programming. Here we will
  introduce `numpy`, especially `numpy` arrays and their built in functions (i.e.
  "methods"). Here, we will also consider how to speed up `numpy` code using the
  `Numba` just-in-time compiler.

* Topic 2: *Data processing with `pandas`*. The `pandas` library provides means to
  represent and manipulate data frames. Like `numpy`, `pandas` can be see as part
  of the de facto standard library for data oriented uses of Python. Here, we will
  focus on data wrangling including selecting rows and columns by name and other
  criteria, applying functions to the selected data, aggregating the data. For this,
  we will use Pandas directly, and also helper packages like `siuba`.

## Day 2

* Topic 3: *Data Visualization*. Python provides many options for data
  visualization.  The `matplotlib` library is a low level plotting library that
  allows for considerable control of the plot, albeit at the price of a
  considerable amount of low level code. Based on `matplotlib`, and providing a
  much higher level interface to the plot, is the `seaborn` library. This allows
  us to produce complex data visualizations with a minimal amount of code.
  Similar to `seaborn` is `ggplot`, which is a direct port of the widely used R
  based visualization library.

* Topic 4: *Statistical data analysis*. In this section, we will describe
  how to perform widely used statistical analysis in Python. Here we will
  start with the `statsmodels`, which provides linear and generalized
  linear models as well as many other widely used statistical models. We
  will also cover `rpy2`, which is and interface from Python to R. This
  allows us to access all of the the power of R from within Python.

* Topic 5: *Symbolic mathematics*. Symbolic mathematics systems, also known as
  computer algebra systems, allow us to algebraically manipulate and solve
  symbolic mathematical expression. In Python, the principal symbolic
  mathematics library is `sympy`. This allows us simplify mathematical
  expressions, compute derivatives, integrals, and limits, solve equations,
  algebraically manipulate matrices, and more.

* Topic 6: *Parallel processing*. In this section, we will cover how to parallelize code to take advantage of multiple processors.
  While there are many ways to accomplish this in Python, here we will focus on the `multiprocessing` package.
