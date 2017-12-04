# Class 26: 2017-12-05

## Today's Slides

Today's Slides are available for download in both [PDF](https://github.com/THOMASELOVE/431slides/blob/master/class_26/431_2017_class-26-slides.pdf) and [R Markdown](https://github.com/THOMASELOVE/431slides/blob/master/class_26/431_2017_class-26-slides.Rmd) formats. 

The audio recording for this class will be posted above as soon as it is available.

## Announcements before class:

1. Today's Agenda
    - Debrief on [Assignment 6](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-6.md)
    - Calibrating Yourself on Residual Plots
    - Modeling the `dm192` data

2. Remaining Course Deliverables
    - [Project Task E](https://github.com/THOMASELOVE/431project/tree/master/TaskE): the final report, due noon Wednesday 2017-12-13.
    - [Project Task F](https://github.com/THOMASELOVE/431project/tree/master/TaskF): the final presentation. The [Schedule](https://github.com/THOMASELOVE/431project/blob/master/TaskF/SCHEDULE.md) is still here.
        - A piece of project presentation advice, in the form of a [Tweet by Roger Peng](https://twitter.com/rdpeng/status/937460535540383744) which I hope will convince you to spend time on drawing effective graphs that **show your data**...
            - "Show me your equations and models and I'll ask to see your data. Show me your data and I won't need to see your equations and models."
            - A nice [follow-up comment](https://twitter.com/joranelias/status/937466061489807360) was "Might still need to tell me how you collected the data, though."
    - **Quiz 3** will be made available on 2017-12-07 by 5 PM and is due at noon on Tuesday **2017-12-12** (*note change*). 
        - The Quiz covers the entire 431 course, emphasizing Part C.
        - Be sure you have completed reading both *The Signal and the Noise* and *The Elements of Data Analytic Style*.
    - **Appealing HW Grades**: If you want me to regrade an assignment, review the [Grade Appeal Policy](https://thomaselove.github.io/431syllabus/general-course-policies.html#grade-appeal-policy---wait-until-december) in the Syllabus, and then request such a regrade by filling out [this Google Form](https://goo.gl/forms/v5zBIuGnrLkbiuXU2) before noon on Wednesday **2017-12-13**.

4. FAQ
    - *How do I convert numerically coded variables so that R treats them as factors?*
        - Consider `plasma$sex <- fct_recode(factor(plasma$sex), "Female" = "2", "Male" = "1")`.
    - *When comparing models, would the ANOVA and AIC ever disagree? If so, then what?*
        - They will certainly disagree, on occasion. They aren't the only options for in-sample comparison - we have adjusted R-square and BIC, for example. Also, we'll often compare models out of sample with tools like MAPE, MSPE and the maximum absolute error.

5. Cool Things 
    - [datapasta](https://github.com/MilesMcBain/datapasta) may be the most useful thing I've seen in weeks. 

## Announcements after class:
 
