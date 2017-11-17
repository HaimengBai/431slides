# Class 23: 2017-11-16

## Today's Slides

Today's Slides are available for download in both [PDF](https://github.com/THOMASELOVE/431slides/blob/master/class_23/431_2017_class-23-slides.pdf) and [R Markdown](https://github.com/THOMASELOVE/431slides/blob/master/class_23/431_2017_class-23-slides.Rmd) formats. 

The audio recording(s) for this class will be posted above when they become available.

## Announcements before class:

1. Today's Agenda
    - Quiz 2
        - [The detailed answer sketch](https://github.com/THOMASELOVE/431slides/blob/master/class_23/431-quiz2-sketch-pw-2017.pdf) is available. 
            - You should have received an email from me including your letter grade on Tuesday. If not, let me know by emailing me **NOW**.
            - Complete grades, item-by-item, for most students [can be found here](https://github.com/THOMASELOVE/431slides/blob/master/class_23/431-2017-quiz2-pw-results-for-most-students.pdf). Be sure to check all 8 pages of the document for your HWID number.
                - If your grade is not on this document, then you are part of a semi-random sample of folks who instead received an email from me today with your detailed item-by-item grade. 
                - Let me know if you can't find your item-by-item grade, either in your email or on the document above.
            - There's an [extra task available](https://goo.gl/forms/1f27voQF33hqYOys1), for those who scored B- or lower. If you did better than a B-, you have the *option* to do the task (before 2017-11-29 at noon) for a little class participation credit.
    - [Class Participation Update through 2017-11-15](https://github.com/THOMASELOVE/431slides/blob/master/class_23/431-class-part-pw-2017-11-15.pdf) 
        - Essentially, you start at 75 and can only go up (remember that a B in 431 usually ranges from 70 - 85, and an A is usually 90 - 100, with 86-89 in the B+/A- range.) 
            - If you're below 85 and worried about it, you probably want to re-introduce yourself to me at some point, both in person and by asking questions or making contributions at 431-help. 
            - Arguing about the score is a waste of your time and mine. Making certain I know who you are is not. I don't know all of your names yet, which is appalling, but true.
            - Note that if you've been visiting TA office hours regularly, that's **not** accounted for yet in this document but will be at the end of the semester.
        - No matter what your score is, I wouldn't worry about it much. Effort on your project will be repaid far more extravagantly than effort towards this measure. 
        - This is the last update on this issue that you'll see. I won't revisit these details again until mid-December.
    - Assignment 5
        - [Answer sketch](https://github.com/THOMASELOVE/431homework/tree/master/HW5) is available in both PDF and R Markdown. 
        - [Grades and the rubric](https://github.com/THOMASELOVE/431homework/tree/master/HW5) are also now available. 
        - There were a lot of problems with attention to detail in the assignment. See the TA comments in the grades sheet.
    - Discussion of the After Class 22 Activity ([Google Form here](https://goo.gl/forms/GEXC4gxQV4aTJb8D3))
        - The activity required you to read [this short primer on p hacking](https://www.methodspace.com/primer-p-hacking/).
        - Andrew Gelman: [What should this student do? His bosses want him to p-hack and they don’t even know it!](http://andrewgelman.com/2017/11/11/student-bosses-want-p-hack-dont-even-know/)
    - Update for the `tidyverse` - [details here](https://www.tidyverse.org/articles/2017/11/tidyverse_1.2.0/) - get version 1.2.1 by updating the tidyverse package in R Studio.
    - Take a look at this Shiny app: [How will the House Tax Bill Impact Graduate Students?](https://benjaminackerman.shinyapps.io/GOPtax2017/) by Benjamin Ackerman. 
        - Want to learn more about Shiny? I hope we'll discuss it in 432, but in the meantime, [take a look at this tutorial](https://shiny.rstudio.com/tutorial/)
    - Modeling in the Tidyverse (Part C of the Course) begins.
        - See [Course Notes](https://thomaselove.github.io/431notes/), sections 37-.

2. The Projects
    - You should be able to do all of your Project related to the Class Survey (Study 1) now.
        - Get the [data and the R Markdown file](https://github.com/THOMASELOVE/431project/tree/master/SURVEY2017) you'll need to clean and rename the data.
        - See the complete [Study 1 demonstration in Task E](https://github.com/THOMASELOVE/431project/tree/master/TaskE) using old survey data ([R Markdown](https://raw.githubusercontent.com/THOMASELOVE/431project/master/TaskE/431-project-study1-demonstration.Rmd) and [PDF](https://github.com/THOMASELOVE/431project/blob/master/TaskE/431-project-study1-demonstration.pdf) available.)
    - [Task D](https://github.com/THOMASELOVE/431project/tree/master/TaskD) is due via email to Dr. Love noon Monday, **2017-11-20**.
        - If you're working with NHANES data, I want to know what tables you used, and I want your cleaned tidied data set, but I don't need the raw pulls.
        - A tidy data set is just a .csv file in almost all cases, rather than multiple .csv files. One .csv file, with one row per subject and one column per variable.
        - **Note**: I expect that **most** people will change their plan described in Task A at least a little in presenting Task D, and certainly Tasks E and F.
        - Your submitted project (Tasks E/F) files should begin by importing a tidy data set and then manipulating the data as needed before you move into the analysis phase. But the data need to be tidy (rows = observations, columns = variables) at the start. 
            - You will build one tidy data file for Study 1 (the class survey data - using the [R Markdown and Excel files I have supplied](https://github.com/THOMASELOVE/431project/tree/master/SURVEY2017)) and another one for Study 2, which is what you are preparing and submitting for Task D.
            - I expect you to use two different Markdown files (one for Study 1 and one for Study 2) to complete Tasks E and F.
        - To date, Project Task D is complete for Chaim Domb, Gwendolyn Donley, Kedar Mahajan, and Roberto Martinez. Thanks!

3. Upcoming non-project Deliverables
    - [Assignment 6](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-6.md) is due at noon **2017-12-01**. Note the big change described in #5 below.

4. The stage version of "**It's a Wonderful Life**" that I play Uncle Billy in has two remaining performances, at 8 PM on Friday Nov 17 and at 8 PM on Saturday Nov 18. It's at [Independence Community Theatre](http://www.independencetheatre.org/) and tickets are available for $12 by calling 216-447-0443. Location: Old Independence Town Hall, 6652 Brecksville Rd, Independence OH. 
    - **PLEASE feel absolutely ZERO obligation to attend**. I mention this so you have the details if you are interested. I would be happy to see you there, but you won't get any extra credit for coming, *nor will I think any less of you should you not attend*.

## Announcements after class:

5. There is an important change in [Assignment 6](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-6.md). In an attempt to ease the burden of the remainder of the course, and to keep the focus where it needs to be (on the project), you will see that **Questions 1 and 6 are no longer part of the assignment**. Instead, you are to do **Questions 2-5**, only.
    - If you have already done work on Question 1 or 6, please feel free to include it and we'll award a little extra credit on the assignment, but if you haven't started on those two questions, then just do questions 2-5. 
    - Any extra time you'd put in to Question 1 or 6 should instead be put towards Quiz 3 and (especially) your project.

6. Be sure to get Project Task D in. It's due at noon Monday 2017-11-20, but Dr. Love will sit down to look at them Tuesday 2017-11-21 at 9 AM, so that is the real drop-dead date. 

7. Remember that our next class is on **Tuesday 2017-11-28**. There will be no TA office hours nor class for my section Thanksgiving Week, but Dr. Love will be available via 431-help on Monday and Tuesday 2017-11-20 and 2017-11-21.
