# Class 22: 2017-11-13

## Today's Slides

Today's Slides are available for download in both [PDF](https://github.com/THOMASELOVE/431slides/blob/master/class_21/431_2017_class-21-slides.pdf) and [R Markdown](https://github.com/THOMASELOVE/431slides/blob/master/class_21/431_2017_class-21-slides.Rmd) formats. 

The audio recording(s) for this class will be posted above when they become available.

## Announcements before class:

1. Today's Agenda
    - Quiz 2
        - due at 8 AM Tuesday 2017-11-14.
    - *p* Hacking, Researcher Degrees of Freedom and The Garden of Forking Paths
        - [Andrew Gelman's blog](http://andrewgelman.com/) is how I first heard about much of this material.
        - The **p-hacking** example I'll show is part of [Science isn't broken](https://fivethirtyeight.com/features/science-isnt-broken/#part1) by Christie Aschwanden with graphic by Ritchie King at FiveThirtyEight.com
        - Some additional references are found [in a talk I gave and its links](https://github.com/THOMASELOVE/RCR2017).
    - What to do about a study after it's published?
        - The retrodesign function, Type S and Type M errors
        - The Gelman and Carlin paper on retrodesign is [here](http://www.stat.columbia.edu/~gelman/research/published/retropower_final.pdf) and two good blog posts on it are [here](http://andrewgelman.com/2016/10/25/how-not-to-analyze-noisy-data-a-case-study/) and also [here](http://andrewgelman.com/2016/11/13/more-on-my-paper-with-john-carlin-on-type-m-and-type-s-errors/)
        - Eric Ravenscraft's piece at Lifehacker on "[How to Lie to Yourself and Others with Statistics](http://lifehacker.com/how-to-lie-to-yourself-and-others-with-statistics-1788184031)" is a fun read.
    - [Course Project Survey Data](https://github.com/THOMASELOVE/431project/tree/master/SURVEY2017), including
        - How To Get It and Clean It Up in R ([get the data and cleanup Markdown here](https://github.com/THOMASELOVE/431project/tree/master/SURVEY2017))
        - What To Do Next: see Project Task E for [detailed demonstrations with old data](https://github.com/THOMASELOVE/431project/tree/master/TaskE)
    - [My reactions to Your Task C work](https://github.com/THOMASELOVE/431project/blob/master/SURVEY2017/TASKC-RESULTS.md)
        - Don't forget to look closely at Canvas for my responses to your work.
        - There's no need to resubmit Task C - just fix your errors and report the new plan as part of Tasks E and F.

2. Coming Soon
    - Assignment 5's [Answer Sketch](https://github.com/THOMASELOVE/431homework/tree/master/HW5) is available. Rubric and grades will come soon.
    - Modeling in the Tidyverse (Part C of the Course) begins next time, in Class 23.
        - See [Course Notes](https://thomaselove.github.io/431notes/), sections 37-.
    
3. The Projects
     - [Task D](https://github.com/THOMASELOVE/431project/tree/master/TaskD) is due via email to Dr. Love noon Monday, **2017-11-20**.
        - If you're working with NHANES data, I want to know what tables you used, and I want your cleaned tidied data set, but I don't need the raw pulls.
        - A tidy data set is just a .csv file in almost all cases, rather than multiple .csv files. One .csv file, with one row per subject and one column per variable.
        - Your submitted project (Tasks E/F) files should begin by importing your tidy data set (from Task D) and then manipulating the data as needed before you move into the analysis phase. But the data need to be tidy at the start. This applies for Study 1 and for Study 2.

4. Upcoming non-project Deliverables
    - [Assignment 6](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-6.md) is due at noon **2017-12-01**.

5. The stage version of "**It's a Wonderful Life**" that I play Uncle Billy in has two remaining performances, at 8 PM on Friday Nov 17 and at 8 PM on Saturday Nov 18. It's at [Independence Community Theatre](http://www.independencetheatre.org/) and tickets are available for $12 by calling 216-447-0443. Location: Old Independence Town Hall, 6652 Brecksville Rd, Independence OH. 
    - **PLEASE feel absolutely ZERO obligation to attend**. I mention this so you have the details if you are interested. I would be happy to see you there, but you won't get any extra credit for coming, *nor will I think any less of you should you not attend*.

## Announcements after class:
