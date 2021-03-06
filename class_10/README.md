**Class 10: 2017-09-28**

## Today's Slides

Today's Slides are available for download in both [PDF](https://github.com/THOMASELOVE/431slides/blob/master/class_10/431_2017_class-10-slides.pdf) and [R Markdown](https://github.com/THOMASELOVE/431slides/blob/master/class_10/431_2017_class-10-slides.Rmd) formats. 

When the audio recording for today's class becomes available, we'll post it above.

## Announcements before class:

1. Today's agenda is focused on working with factors (using some of the VHL data) then on building tables, dealing with missingness, and building scatterplot and correlation matrices, all using the data from the Western Collaborative Group Study, from Section 13 of the [Course Notes](https://thomaselove.github.io/431notes/index.html). 

We'll build the **Task B groups for the project** as our first activity, though. Your Task B group will submit its information via this [Google Form](https://goo.gl/forms/WaQOdCEAW0wxdjJh2) by *5 PM* on **Thursday, 2017-09-28**. 2 groups of 4 have already done so. If you are a group of less than 5 people, I may assign you a fifth member, so go for 5.

2. [Assignment 3](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-3.md) is due at noon on Friday **2017-09-29**. 

Some common issues:
- If one of us answers your question, great. But if you have to write back to clarify, it helps if you can override your email's wish to reply just to the individual email of the person who answered your question and instead send your follow-up back to 431-help.
- If you're looking for a model for Question 5, consider a close look at Section 11.4.3 of [the Notes](https://thomaselove.github.io/431notes/index.html).
- When fitting a loess smooth, in Question 7, for instance, in the aes part of your ggplot call, you don't need to specify group = Species, if you've already got color = Species. If you do, the loess won't work well, although the lm will.
- Sometimes R will throw an error saying that a particular package is missing. This is usually because some package that the tidyverse (or some other package you're trying to load) uses has been updated. Updating your packages can help, especially after closing R Studio and restarting, or try just reinstalling the missing package, by visiting Packages in the bottom right window, and selecting Install packages, then specifying the name of the missing piece.

3. Today, we'll take a peek at some of the functions in the [broom package](https://cran.r-project.org/web/packages/broom/vignettes/broom.html), which I've just added to the list of [packages you should install](https://github.com/THOMASELOVE/431/blob/master/software-installation-431.md).

4. For Class 11 (2017-10-03), please:

- Read Ehrenberg's [The Problem of Numeracy](https://github.com/THOMASELOVE/431slides/blob/master/class_10/Ehrenberg_1981_pw_The_Problem_of_Numeracy.pdf). The file is password-protected, but not actually invalid as GitHub suggests.
- Read Jeff Leek's *Elements of Data Analytic Style* Chapters 1-4 and 12.
- We'll have a Project Task B meeting on Tuesday 2017-10-03, as well, so it would be helpful to read over the [material on Task B](https://github.com/THOMASELOVE/431project/tree/master/TaskB) before class.
- You should be finished reading Part A of the [Course Notes](https://thomaselove.github.io/431notes/) by now.
- You should also be finishing up the **Explore** and **Wrangle** material in [R For Data Science](http://r4ds.had.co.nz/).

5. Upcoming Readings/Assignments/Deadlines:

- [Quiz 1](https://thomaselove.github.io/431syllabus/quizzes.html) will come to you on 2017-10-05 and is due at noon on **2017-10-09**.
- Read Nate Silver's *The Signal and the Noise* Chapters 4 and 5 (Weather and Earthquake Predictions) [as well as Jeff Leek's Chapter 6] by **2017-10-10**, and Silver's Chapters 7 and 8 (Disease Outbreaks and Bayes' Theorem) by **2017-10-17**.
- [Project Task A](https://github.com/THOMASELOVE/431project/tree/master/TaskA) is due at noon on **2017-10-13**.
- [Assignment 4](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-4.md) is due at noon on **2017-10-20**.
- [Project Task B](https://github.com/THOMASELOVE/431project/tree/master/TaskB) is due at noon on **2017-10-23**. Time will be available in class for 15-20 minute group meetings on **2017-10-03** and **2017-10-12**.

## Announcements after class:

6. Don't forget about Assignment 3 due tomorrow. See the comments in #2 above.
