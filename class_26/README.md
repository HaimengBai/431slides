# Class 26: 2017-12-05

## Today's Slides

Today's Slides are available for download in both [PDF](https://github.com/THOMASELOVE/431slides/blob/master/class_26/431_2017_class-26-slides.pdf) and [R Markdown](https://github.com/THOMASELOVE/431slides/blob/master/class_26/431_2017_class-26-slides.Rmd) formats. 

The audio recording for this class will be posted above as soon as it is available.

## Announcements before class:

1. Today's Agenda
    - Debrief on [Assignment 6](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-6.md).
        - Answer sketch and rubric [are here](https://github.com/THOMASELOVE/431homework/tree/master/HW6) now.
    - Roger Peng's comments on Reasoning About Data [blog post 1](https://simplystatistics.org/2017/11/16/reasoning-about-data/) and [blog post 2](https://simplystatistics.org/2017/11/20/follow-up-on-reasoning-about-data/)
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
        - Another tip for your Project and the Quiz is to familiarize yourself with some of the functions from the `forcats` package: fct_relevel`, `fct_collapse`, `fct_relevel`, `fct_lump`, and `fct_reorder` for instance.
            - Confronted with a situation where you need to adjust a factor, these are all useful.
            - Consider looking at Jenny Bryan's [Stat545 notes on factors](http://stat545.com/block029_factors.html)
            - You might also consider reading the Factors chapter of [R for Data Science](http://r4ds.had.co.nz/factors.html).
    - **Appealing HW Grades**: If you want me to regrade an assignment, review the [Grade Appeal Policy](https://thomaselove.github.io/431syllabus/general-course-policies.html#grade-appeal-policy---wait-until-december) in the Syllabus, and then request such a regrade by filling out [this Google Form](https://goo.gl/forms/v5zBIuGnrLkbiuXU2) before noon on Wednesday **2017-12-13**.

4. FAQ
    - *Should I name my data set* `data`? *Should I name my model* `model`?
        - Never. Never ever ever do this.
        - Always grant a specific name to any object worth storing. 
        - If you have a kitchen sink model for Question 3, at least name it `model_ks_3`.
    - *The code runs step-by-step, but doesn't work when I try to knit the whole file*
        - Have you checked your YAML code at the beginning of the document to be sure it says what it should and no more? 
        - Every detail matters.
    - *Which packages should I load, and in what order should I load them?*
        - I expect most people will need to load `car`, `broom` and `tidyverse`, in that order, for regression modeling.
        - You may need to load other packages, but DON'T load anything you don't actually need to load. 
            - If the only thing you'll use mosaic for is `favstats`, for instance, don't load it, just type `mosaic::favstats` when you want to call that function. 
            - The only good thing loading a package does is eliminate the need to type `nameofpackage::nameoffunction` when you want to run a function from that package.
            - The bad things loading a package can do may be substantial.
            - It is **important** to put the tidyverse last, and then (after loading all packages) source in `Love-boost.R`
    - *How do I convert numerically coded variables so that R treats them as factors?*
        - Consider `plasma$sex <- fct_recode(factor(plasma$sex), "Female" = "2", "Male" = "1")`.
    - *When comparing models, would the ANOVA and AIC ever disagree? If so, then what?*
        - They will certainly disagree, on occasion. They aren't the only options for in-sample comparison - we have adjusted R-square and BIC, for example. Also, we'll often compare models out of sample with tools like MAPE, MSPE and the maximum absolute error.
    - *I'm having trouble inserting the image HW6pic.png into my R Markdown file.*
        - I suggest you try the `include_graphics` function which is part of the `knitr` package.
        - Typing the following into its own (echo = F) R code chunk may solve your problem: `knitr::include_graphics("HW6pic.png")`
    - *Should I upgrade to R 3.4.3 now that it's becoming available?*
        - You are welcome to do so, but I would probably wait until either (a) a needed package wouldn't load under an earlier version of R, or (b) your project and Quiz 3 are complete.
    - *How do I get a GitHub user name? What should I choose as my name?*
        - Jenny Bryan has some sage advice about GitHub usernames and the process at [Happy Git With R](http://happygitwithr.com/github-acct.html)

5. Cool Things 
    - [datapasta](https://github.com/MilesMcBain/datapasta) may be the most useful thing I've seen in weeks. 
    - Jeff Leek shares [A few things that would reduce stress around reproducibility/replicability in science](https://simplystatistics.org/2017/11/21/rr-sress/)

## Announcements after class:
 
