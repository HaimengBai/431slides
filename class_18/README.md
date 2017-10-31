# Class 18: 2017-10-31

## Today's Slides

Today's Slides are available for download in both [PDF](https://github.com/THOMASELOVE/431slides/blob/master/class_18/431_2017_class-18-slides.pdf) and [R Markdown](https://github.com/THOMASELOVE/431slides/blob/master/class_18/431_2017_class-18-slides.Rmd) formats. 

When the audio recording for today's class becomes available, we'll post it above.

## Announcements before class:

1. Today's Agenda
    - Discussion of the In-Class Survey from Class 17. Again, those questions were:
        - We chose (using a computer) a random number between 0 and 100. Your number is X = 10 (or 65).
            1. Do you think the percentage of countries which are in Africa, among all those in the United Nations, is higher or lower than X?
            2. Give your best estimate of the percentage of countries which are in Africa, among all those in the United Nations. (*There are 193 sovereign states that are members of the UN. The African regional group has 54 member states, so that's 28%*)
            3. Provide a point estimate for Dr. Love’s current weight (in pounds.) 
            4. Now estimate one interval, which you believe has a 50% chance of including Dr. Love’s current weight (again, in pounds.) Then do the same for a 90% interval.
    - Analysis of Variance for Comparing More than Two Means [Course Notes](https://thomaselove.github.io/431notes/) Section 28, in particular.
    
2. The Projects
    - Every group has now reviewed the survey, and I've responded via email regarding all requests. Thanks.
        - Items that I changed (most quite lightly) were 36-37, 39, 44, 47, 68, 69. 
            - The biggest change was to item 39, which now asks for the % of all of the money you spent in the past month that you spent online, rather than for the total amount spent online.
            - I clarified the other items above in more detailed descriptions.
            - Some items originally planned as Likert scales are instead on 0-100 scales, but you can categorize those as you like (even to binary variables, in preparing your analyses and your Task C work.
     - [Task C](https://github.com/THOMASELOVE/431project/tree/master/TaskC) will be due at noon on Wednesday, **2017-11-08**. 
        - The Class Survey is [now available as a Google Form](https://goo.gl/forms/bB1xJ16NnLihP9Gu1) accepting responses.
        - You **also need** to submit [this Word template](https://github.com/THOMASELOVE/431project/blob/master/TaskC/2017_task_C_template_for_YOUR_NAME.docx) via Canvas by noon on 2017-11-08. [A PDF version](https://github.com/THOMASELOVE/431project/blob/master/TaskC/2017_What-does-the-Project-Task-C-template-look-like.pdf) is also available so you can see what is required.
        - Details on the scales used in the survey and how they will be included in the project data [are available, too]((https://github.com/THOMASELOVE/431project/blob/master/TaskC/SCALES.md).
    - **NEW DATE** [Task D](https://github.com/THOMASELOVE/431project/tree/master/TaskD) is due via email to Dr. Love noon Monday, **2017-11-20**.
        - Many of you could do this task **right now** to get ahead of things a bit. Note that this is a **corrected** date.

3. Upcoming non-project Deliverables
    - **NEW DATE** In a change, [Assignment 5](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-5.md) is now due at noon on Thursday **2017-11-09**. This is delayed six days, so it is now the day after Project Task C is due.
        - Note that you should be able to do questions 1 and 5-10 after we've finished our ANOVA discussions, but that questions 2-4 will require some discussion in class of comparing rates/proportions, and that'll begin on Thursday, in Class 19.
    - Read Silver, through Chapter 11 by 2017-11-02.
    - Quiz 2 will be released on Thursday 2017-11-09 by 5 PM and is due on Monday **2017-11-13** at noon.
        - To help with your review, a brief [additional example on key Part A material](https://github.com/THOMASELOVE/431homework/tree/master/Extra_A) is available. 
        - **NEW** An [Answer Sketch](https://github.com/THOMASELOVE/431homework/blob/master/Extra_A/extra_A.pdf) is now available, too.
    - Leek, Chapters 7-8 should be read by 2017-11-14.
    - Silver Chapter 12 by 2017-11-28, and finish the book by 2017-12-05.

4. The [Assignment 4 Answer Sketch](https://github.com/THOMASELOVE/431homework/blob/master/HW4/README.md) is now available in both R Markdown and (password-protected) PDF.

5. Some Tips
    - **Use R Projects.** I cannot emphasize enough how important it is to use R Projects in R Studio. Your first step in any analysis should be to create a new Project in a clean directory on your computer, in which you'll store your data, markdown files, etc. I have a separate project for each class, for each homework assignment, for the Course Project. If you're storing everything from the whole course in one place, without any subdirectories, it will be a real challenge if you start having problems. Using [R Projects](https://support.rstudio.com/hc/en-us/articles/200526207-Using-Projects) certainly gets R to default to a sensible choice of directory, which is already a big help. But it has [several other advantages](https://swcarpentry.github.io/r-novice-gapminder/02-project-intro/), too. When you have projects that are more substantial - not just one data set, not just one analysis (as the homework lulls you into developing) using a project will make your life considerably easier.
    - **Visualization "do and don't" advice.** The big advantage of using ggplot2 and the tidyverse more generally is that it's easier to fall into a good plot as long as you tidy your data appropriately. For some advice on visualizing data more effectively, I recommend [this guide by Jenny Bryan](http://stat545.com/block015_graph-dos-donts.html) and its list of resources, which include [these materials from Karl Broman](https://github.com/kbroman/Talk_Graphs). 
    - **Jenny Bryan is a name you want to know.** Incidentally, a good pro tip (from [Michael Lopez on Twitter](https://twitter.com/StatsbyLopez/status/916348419547062272/photo/1)) is that when you're searching for help on using R, add Jenny Bryan at the end. In a crowded universe of advice on programming well, her materials are always outstanding. 
    
## Announcements after class:

6. [Slides have been reposted for Class 18](https://github.com/THOMASELOVE/431slides/blob/master/class_18/431_2017_class-18-slides.pdf), to include only those things we actually discussed and to correct typos.

7. I've [reposted the Sketch and added the Rubric](https://github.com/THOMASELOVE/431homework/tree/master/HW4) for Assignment 4. The assignment has 145 points available, in total, not 150.
