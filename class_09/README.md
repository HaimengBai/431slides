**Class 9: 2017-09-26**

## Today's Slides

Today's Slides are available for download in both [PDF](https://github.com/THOMASELOVE/431slides/blob/master/class_09/431_2017_class-09-slides.pdf) and [R Markdown](https://github.com/THOMASELOVE/431slides/blob/master/class_09/431_2017_class-09-slides.Rmd) formats. 

When the audio recording for today's class becomes available, we'll post it above.

## Announcements before class:

1. The main material from the [Course Notes](https://thomaselove.github.io/431notes/) today refers to Associations and Using Linear Models (Chapter 11) as demonstrated using a study of von Hippel-Lindau disease. [Von Hippel-Lindau syndrome](http://www.cancer.net/cancer-types/von-hippel-lindau-syndrome) (VHL) is a hereditary condition associated with tumors arising in multiple organs. Today's agenda also includes
  + discussion of Chapters 2 and 3 of The Signal and the Noise
  + some discussion of [Assignment 2](https://github.com/THOMASELOVE/431homework/blob/master/HW2/README.md)

2. **gg_qq is no more.** The [Course Notes](https://thomaselove.github.io/431notes/index.html) (in several places) used to use the `gg_qq` plot approach that is part of Love-boost.R. But that doesn't work so well (in particular, it has trouble with missing data, doesn't allow you to adjust the title easily, and cannot be incorporated easily into multiple plot arrays.) So, this weekend I removed the references to `gg_qq` and replaced them with regular `ggplot` approaches using the `geom_qq` geom, and with base graphics approaches using `qqnorm` and `qqline`. The affected sections are 8.5 and 8.6. I have also updated the answer sketch for Assignment 2 to replace `gg_qq` with other ggplot-based approaches.

3. Upcoming Readings/Assignments/Deadlines:

- You should finish reading Part A of the [Course Notes](https://thomaselove.github.io/431notes/) by the end of this month.
- I also suggest working your way through [R For Data Science](http://r4ds.had.co.nz/). All of the **Explore** and **Wrangle** material is likely to be helpful in Part A of the course.
- Read Jeff Leek's *Elements of Data Analytic Style* Chapters 1-4 and 12 by **2017-10-03**.
- [Quiz 1](https://thomaselove.github.io/431syllabus/quizzes.html) will come to you on 2017-10-05 and is due at noon on **2017-10-09**.
- Read Nate Silver's *The Signal and the Noise* Chapters 4 and 5 (Weather and Earthquake Predictions) [as well as Jeff Leek's Chapter 6] by **2017-10-10**, and Silver's Chapters 7 and 8 (Disease Outbreaks and Bayes' Theorem) by **2017-10-17**.
- [Project Task A](https://github.com/THOMASELOVE/431project/tree/master/TaskA) is due at noon on **2017-10-13**.
- [Assignment 4](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-4.md) is due at noon on **2017-10-20**.
- [Project Task B](https://github.com/THOMASELOVE/431project/tree/master/TaskB) is due at noon on **2017-10-23**. Time will be available in class for 15-20 minute group meetings on **2017-10-03** and **2017-10-12**.

## Announcements after class:

4. Change of plans. We'll build the Task B groups as our first activity on Thursday (Class 10). Your Task B group will submit its information via this [Google Form](https://goo.gl/forms/WaQOdCEAW0wxdjJh2) by *5 PM* on **Thursday, 2017-09-28**. Thanks.

5. Audio files are now posted for Class 9.

6. Don't forget that [Assignment 3](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-3.md) is due Friday 2017-09-29.

