# Class 26: 2017-12-05

## Today's Slides

Today's Slides are available for download in both [PDF](https://github.com/THOMASELOVE/431slides/blob/master/class_26/431_2017_class-26-slides.pdf) and [R Markdown](https://github.com/THOMASELOVE/431slides/blob/master/class_26/431_2017_class-26-slides.Rmd) formats. 

The audio recordings for this class are posted above.

## Announcements before class:

1. Today's Agenda
    - Debrief on [Assignment 6](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-6.md).
        - Answer sketch and rubric [are here](https://github.com/THOMASELOVE/431homework/tree/master/HW6) now.
    - Roger Peng's comments on Reasoning About Data [blog post 1](https://simplystatistics.org/2017/11/16/reasoning-about-data/) and [blog post 2](https://simplystatistics.org/2017/11/20/follow-up-on-reasoning-about-data/)
    - Calibrating Yourself on Residual Plots
    - Modeling the `dm192` data

2. Remaining Course Deliverables
    - There is a short [Task after Class 26](https://goo.gl/forms/0YAdfGQIufanWSnG2) online now. I would really appreciate it if you would complete this before 9 AM on Thursday 2017-12-07.
    - [Project Task E](https://github.com/THOMASELOVE/431project/tree/master/TaskE): the final report, due noon Wednesday 2017-12-13.
    - [Project Task F](https://github.com/THOMASELOVE/431project/tree/master/TaskF): the final presentation. The [Schedule](https://github.com/THOMASELOVE/431project/blob/master/TaskF/SCHEDULE.md) is still here.
        - A piece of project presentation advice, in the form of a [Tweet by Roger Peng](https://twitter.com/rdpeng/status/937460535540383744) which I hope will convince you to spend time on drawing effective graphs that **show your data**...
            - "Show me your equations and models and I'll ask to see your data. Show me your data and I won't need to see your equations and models."
            - A nice [follow-up comment](https://twitter.com/joranelias/status/937466061489807360) was "Might still need to tell me how you collected the data, though."
    - **Quiz 3** will be made available on 2017-12-07 by 5 PM and is due at noon on Tuesday **2017-12-12** (*note change*). 
        - The Quiz covers the entire 431 course, emphasizing Part C.
        - Be sure you have completed reading both *The Signal and the Noise* and *The Elements of Data Analytic Style*.
        - Another tip for your Project and the Quiz is to familiarize yourself with some of the functions from the `forcats` package: fct_recode`, `fct_collapse`, `fct_relevel`, `fct_lump`, and `fct_reorder` for instance.
            - Confronted with a situation where you need to adjust a factor, these are all useful.
            - Consider looking at Jenny Bryan's [Stat545 notes on factors](http://stat545.com/block029_factors.html)
            - You might also consider reading the Factors chapter of [R for Data Science](http://r4ds.had.co.nz/factors.html).
    - **Appealing HW Grades**: If you want me to regrade an assignment, review the [Grade Appeal Policy](https://thomaselove.github.io/431syllabus/general-course-policies.html#grade-appeal-policy---wait-until-december) in the Syllabus, and then request such a regrade by filling out [this Google Form](https://goo.gl/forms/v5zBIuGnrLkbiuXU2) before noon on Wednesday **2017-12-13**.
    - **Course Evaluations** You will get at least two evaluations for this course. The official one from the University should be in your email already. Please complete it. It's important. I will also ask you to fill out one for me about specific details of the class, soon. 

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
    - *Do I need to rerun [a] checks for collinearity or [b] residual plots after I use stepwise regression to select variables and fit a smaller model than my original (kitchen sink) model?*
        - Assessments of model assumptions (which include linearity, constant variance, independence and Normality) are critical steps in every regression setting. Re-assessing assumptions is necessary for every new model. So looking at residual plots is necessary after using, for instance, a stepwise approach to select variables from a larger model for a new model.
        - Assessments of collinearity are less crucial, and are mostly necessary when we believe that two or more predictors may be strongly correlated with one another, and we want to tease out the nature of the relationships between our outcome and each predictor separately. But if you don't have a collinearity problem in a large model (like a kitchen sink), you won't have collinearity issues in a model that uses just a subset of the predictors in your large model.
    - *What is the role of collinearity checks?*
        - Collinearity is what statisticians call the situation when we are running a prediction model and several of the predictors are correlated with each other. Generically, if we think of an outcome Y being predicted by X1, X2 and X3, then collinearity is what happens when, for example, X1 and X2 are highly correlated with each other. If collinearity is large enough, the regression model will still work, but it will be very difficult for us to separate out the predictive power of X1 from the predictive power of X2, which can lead to problems interpreting our model.
            - In 431, we investigate whether collinearity is a problem using the VIF statistic (VIF = variance inflation factor). If the VIF for one or more predictors is larger than 5, we have problematic collinearity.
            - If we see one or more VIF values greater then 5, our first solution is typically to drop one of the "large VIF" predictors from our model - often, we'll figure this out by looking at a t test.
            - If the collinearity is large enough, then when we drop a predictor, we should see some improvement (decrease) in the VIF statistics and we may also see the t test p values for some predictors fall, too.
    - *What is the role of outcome transformation in regression?*
        - Transformation of an outcome is necessary when our outcome does not have a linear relationship with the set of predictors we are interested in. If we have a non-linearity problem, that is a serious violation of the assumptions of a linear regression model, and our predictions will be poor, as a result. 
            - In 431, we investigate whether the non-linearity assumption is violating by plotting a model's residuals against its fitted values, and look for a curve. If we find one, a transformation of the outcome is a possible solution.
            - Problems with non-constant variance (indicated by a fan in the residuals vs. fitted values plot) or with skew in the residuals (as shown in a Normal Q-Q plot of the residuals) may also be amenable to a potential transformation of the outcome.
            - To help us decide what transformation might be most appropriate in a given circumstance, we can use the Box-Cox tool to assess a variety of power transformations quickly (so long as our outcome Y is strictly positive) and give us an indication as to which of several common transformations (including the log, square root, inverse and square) might be most helpful.
            - Should our outcome variable not be Normally distributed in building a model, we might also consider a transformation, also motivated by Box-Cox, in an effort to reduce the likelihood of serious non-Normality in our residuals.
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

6. A reminder that there is a short [Task after Class 26](https://goo.gl/forms/0YAdfGQIufanWSnG2) Google Form online. I would really appreciate it if you would complete this before **9 AM on Thursday 2017-12-07**. Thanks in advance.

7. I've changed the Project Task E instructions to ask you to submit your work via Canvas, rather than email, and to reflect the reality that you don't need to merge the survey files into a new .csv in Study 1, so that no Study 1 data set needs to be submitted.


