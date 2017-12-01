# Class 25: 2017-11-30

## Today's Slides

Today's Slides are available for download in both [PDF](https://github.com/THOMASELOVE/431slides/blob/master/class_25/431_2017_class-25-slides.pdf) and [R Markdown](https://github.com/THOMASELOVE/431slides/blob/master/class_25/431_2017_class-25-slides.Rmd) formats. 

The audio recording(s) for this class will be posted above when they become available.

## Announcements before class:

1. Today's Agenda
    - Activity After Class 24 - see the [Most Important/Muddiest Results and some Comments on Project Titles](https://github.com/THOMASELOVE/431slides/blob/master/class_25/after24.md).
        - [Here's a quick pdf](https://github.com/THOMASELOVE/431slides/blob/master/class_25/project_confidence.pdf) regarding your self-reported confidence in your project. There's an R Markdown file, too.
    - Stepwise Regression (via Backward Elimination) in the `nyfs2` data
        - Comparing the "Kitchen Sink" model to a Reduced Model
        - Assessing collinearity with the generalized Variance Inflation Factor
        - Assessing assumptions with residual plots
    - Studying Ginzberg's Depression Data (from the `car` package)
        - Selecting a transformation for our outcome
        - Working with standardized predictors/outcomes in regression
        - Partitioning into Test and Training Samples
        - Comparing Models In-Sample with R-squared, AIC, BIC
        - Comparing Model Predictions Out of Sample with MAPE and MSPE for Validation
    - *Getting Better Calibrated on Residual Plots* (**MOVED to Class 26**)
        - Assumption Checking: Linearity, Homoscedasticity, Normality
        - Residuals, Leverage and Influence
        - Six Simulated Situations to Mull Over

2. The Projects
    - [Project Task E](https://github.com/THOMASELOVE/431project/tree/master/TaskE): the final report, due noon Wednesday 2017-12-13.
        - We updated the [Study 2 demonstration](https://github.com/THOMASELOVE/431project/tree/master/TaskE) to fix the coefficient of tobaccoquit on the bottom of page 16.
    - [Project Task F](https://github.com/THOMASELOVE/431project/tree/master/TaskF): the final presentation. [Project Schedule is here](https://github.com/THOMASELOVE/431project/blob/master/TaskF/SCHEDULE.md).

3. Non-project Deliverables
    - [Assignment 6](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-6.md), due noon Monday **2017-12-04**. The assignment is only Questions 2-5. Our [grading rubric](https://github.com/THOMASELOVE/431homework/blob/master/HW6/README.md) may be helpful to you, as will the Project Study 2 Demonstration, available in [PDF](https://github.com/THOMASELOVE/431homework/blob/master/HW6/README.md) and [R Markdown](https://github.com/THOMASELOVE/431project/blob/master/TaskE/431-project-study2-demonstration.Rmd). 
    - **Quiz 3** will be made available on 2017-12-07 by 5 PM and is due at noon on Monday 2017-12-11. It covers the entire 431 course.
    - **Appealing HW Grades**: If you want me to regrade an assignment, review the [Grade Appeal Policy](https://thomaselove.github.io/431syllabus/general-course-policies.html#grade-appeal-policy---wait-until-december) in the Syllabus, and then request such a regrade by filling out [this Google Form](https://goo.gl/forms/v5zBIuGnrLkbiuXU2) before noon on 2017-12-13.

4. Miscellany
    - Amelia McNamara has a [great post on statistics graduate school advice](http://www.science.smith.edu/~amcnamara/blog/teaching/2016/10/19/GradSchool.html), which may have some relevant features for you, even if statistics isn't your primary field.
    - Gelman blog: [Dear Professor Gelman, I thought you would be interested in these awful graphs I found in the paper today](http://andrewgelman.com/2017/11/26/dear-professor-gelman-thought-interested-awful-graphs-found-paper-today/). The [original article](https://www.memphisflyer.com/NewsBlog/archives/2016/08/26/report-alcohol-crashes-down-distracted-driving-accidents-up) from the *Memphis Flyer* includes several other "infographics." Yikes.
    - *Nature* had an interesting commentary Tuesday from six prominent statisticians (including Jeff Leek and Andy Gelman) on [Five ways to fix statistics](https://www.nature.com/articles/d41586-017-07522-z?utm_source=FBK_NatureNews&sf174540015=1). I expect to read this together in 432. 
    

## Announcements after class:
 
5. Course Notes updated again to fix a typo in Section 22.6.1 (removed the word not)

6. Good luck on Assignment 6 (due Mon 2017-12-04), and have a nice weekend. Here's a little help:

*Dear 431 staff: In the HW6 "plasma" dataset, the variables "sex" "smoking" and "vitamin" are coded numerically, despite the fact that they are categorical variables. I have gone through both the course slides and the course notes, but I can't find a way to convert these numeric variables to categorical ones.*

Perhaps you might want to try something like: `plasma$sex <- fct_recode(factor(plasma$sex), "Female" = "2", "Male" = "1")`

