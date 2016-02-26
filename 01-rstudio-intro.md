---
layout: page
title: R for reproducible scientific analysis
subtitle: Introduction to R and RStudio
minutes: 45
---



> ## Learning Objectives {.objectives}
>
> * To gain familiarity with the various panes in the RStudio IDE
> * To gain familiarity with the buttons, short cuts and options in the RStudio IDE
> * To understand variables and how to assign to them
> * To be able to manage your workspace in an interactive R session
> * To be able to use mathematical and comparison operations
> * To be able to call functions
> 

## Introduction to RStudio

Welcome to the R portion of the Software Carpentry workshop.

Throughout this lesson, we're going to teach you some of the fundamentals of
the R language as well as some best practices for organising code for
scientific projects that will make your life easier.

We'll be using RStudio: a free, open source R integrated development
environment. It provides a built in editor, works on all platforms (including
on servers) and provides many advantages such as integration with version
control and project management.

**Basic layout**

When you first open RStudio, you will be greeted by three panels:

  * The interactive R console (entire left)
  * Workspace/History (tabbed in upper right)
  * Files/Plots/Packages/Help (tabbed in lower right)

Once you open files, such as R scripts, an editor panel will also open
in the top left.

## Work flow within RStudio
There are two main ways one can work within RStudio.

1. Test and play within the interactive R console then copy code into
a .R file to run later. 
   *  This works well when doing small tests and initially starting off.
   *  It quickly becomes laborious
2. Start writing in an .R file and use RStudio's command / short cut
to push current line, selected lines or modified lines to the
interactive R console. 
   * This is a great way to start; all your code is saved for later
   * You will be able to run the file you create from within RStudio
   or using R's `source()`  function.

> ## Tip: Running segments of your code {.callout}
>
> RStudio offers you great flexibility in running code from within the editor
> window. There are buttons, menu choices, and keyboard shortcuts. To run the
> current line, you can 1. click on the `Run` button just above the editor panel,
> or 2. select "Run Lines" from the "Code" menu, or 3. hit Ctrl-Enter in Windows
> or Linux or Command-Enter on OS X. (This shortcut can also be seen by hovering
> the mouse over the button). To run a block of code, select it and then `Run`.
> If you have modified a line of code within a block of code you have just run,
> there is no need to reselct the section and `Run`, you can use the next button
> along, `Re-run the previous region`. This will run the previous code block
> inculding the modifications you have made.

## Introduction to R

Much of your time in R will be spent in the R interactive
console. This is where you will run all of your code, and can be a
useful environment to try out ideas before adding them to an R script
file. This console in RStudio is the same as the one you would get if
you just typed in `R` in your commandline environment.

The first thing you will see in the R interactive session is a bunch
of information, followed by a ">" and a blinking cursor. In many ways
this is similar to the shell environment you learned about during the
shell lessons: it operates on the same idea of a "Read, evaluate,
print loop": you type in commands, R tries to execute them, and then
returns a result.


## R Packages

It is possible to add functions to R by
obtaining a package written by someone else. As of this writing, there
are over 7,000 packages available on CRAN (the comprehensive R archive
network). R and RStudio have functionality for managing packages:

* You can see what packages are installed by typing
  `installed.packages()`
* You can install packages by typing `install.packages("packagename")`,
  where `packagename` is the package name, in quotes.
* You can update installed packages by typing `update.packages()`
* You can remove a package with `remove.packages("packagename")`
* You can make a package you have installed available for use in your session with `library(packagename)`

Install the following packages: `ggplot2`, `plyr`, `gapminder`
