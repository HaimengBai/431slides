# Class 23: 2017-11-16

## Today's Slides

Today's Slides are available for download in both [PDF](https://github.com/THOMASELOVE/431slides/blob/master/class_23/431_2017_class-23-slides.pdf) and [R Markdown](https://github.com/THOMASELOVE/431slides/blob/master/class_23/431_2017_class-23-slides.Rmd) formats. 

The audio recording(s) for this class will be posted above when they become available.

## Announcements before class:

1. Today's Agenda
    - Quiz 2
        - [The detailed answer sketch](https://github.com/THOMASELOVE/431slides/blob/master/class_23/431-quiz2-sketch-pw-2017.pdf) are available. 
            - You should have received an email from me about your grade. If not, let me know by emailing me NOW.
            - There's an [extra task available](https://goo.gl/forms/1f27voQF33hqYOys1), for those who scored B- or lower. If you did better than a B-, you have the option to do the task (before 2017-11-29 at noon) for a little class participation credit.
    - [Class Participation Update through 2017-11-15](https://github.com/THOMASELOVE/431slides/blob/master/class_23/431-class-part-pw-2017-11-15.pdf): Essentially, you start at 75 and can only go up (remember that a B in 431 usually ranges from 70 - 85, and an A is usually 90 - 100, with 86-89 in the B+/A- range.) A few people are already at 100 (the max). Some are still at 75.
        - If you're below 85 and worried about it, you probably want to re-introduce yourself to me at some point, both in person and by asking questions or making contributions at 431-help. But I wouldn't worry about it too much, no matter what your score is to date.
        - This won't be updated again until mid-December.
    - Assignment 5
        - Answer sketch and grades are now available.
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
        - Your submitted project (Tasks E/F) files should begin by importing your tidy data set (from Task D) and then manipulating the data as needed before you move into the analysis phase. But the data need to be tidy at the start. 
            - You will build one tidy data file for Study 1 (the class survey data - using the [R Markdown and Excel files I have supplied](https://github.com/THOMASELOVE/431project/tree/master/SURVEY2017)) and the one for Study 2 you prepare and submit for Task D.
            - I expect you to use two different Markdown files (one for Study 1 and one for Study 2.)
        - To date, Project Task D is complete for Chaim Domb, Gwendolyn Donley, Kedar Mahajan, and Roberto Martinez. Thanks!

3. Upcoming non-project Deliverables
    - [Assignment 6](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-6.md) is due at noon **2017-12-01**.

4. The stage version of "**It's a Wonderful Life**" that I play Uncle Billy in has two remaining performances, at 8 PM on Friday Nov 17 and at 8 PM on Saturday Nov 18. It's at [Independence Community Theatre](http://www.independencetheatre.org/) and tickets are available for $12 by calling 216-447-0443. Location: Old Independence Town Hall, 6652 Brecksville Rd, Independence OH. 
    - **PLEASE feel absolutely ZERO obligation to attend**. I mention this so you have the details if you are interested. I would be happy to see you there, but you won't get any extra credit for coming, *nor will I think any less of you should you not attend*.

## Announcements after class:
