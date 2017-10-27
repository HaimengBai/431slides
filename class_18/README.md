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
            3. Provide a point estimate for Dr. Love’s current weight (in pounds.) (*On 2017-10-26, Dr. Love actually weighed 350 lbs. or 158.8 kg or 25 stone, dressed but without shoes.*)
            4. Now estimate one interval, which you believe has a 50% chance of including Dr. Love’s current weight (again, in pounds.) Then do the same for a 90% interval.
    - Analysis of Variance for Comparing More than Two Means [Course Notes](https://thomaselove.github.io/431notes/) Section 28, in particular.
    - Some Thoughts on Statistical Significance and *p* values. References for today include:
        - Jason T. Connor (2004) [The Value of a p-valueless paper](https://www.nature.com/ajg/journal/v99/n9/pdf/ajg2004321a.pdf?origin=ppub)
        - Mark, Lee, and Harrell (2016) [Understanding the Role of P Values and Hypothesis Tests in Clinical Research](https://jamanetwork.com/journals/jamacardiology/article-abstract/2566171)
        - Thomas and Pencina (2016) [Do Not Over (P) Value Your Research Article](https://jamanetwork.com/journals/jamacardiology/fullarticle/2566166)
        - Gelman, Andrew [blog post 2016-10-15](http://andrewgelman.com/2016/10/15/marginally-significant-effects-as-evidence-for-hypotheses-changing-attitudes-over-four-decades/)
    - (if time permits) *The Signal and The Noise*, Chapters 7 and 8
    
2. The Projects
    - [Task C](https://github.com/THOMASELOVE/431project/tree/master/TaskC) will be due at noon on Wednesday, **2017-11-08**. 
        - We hope to make the Class Survey available by 2017-10-30.
    - [Task D](https://github.com/THOMASELOVE/431project/tree/master/TaskD) is due via email to Dr. Love noon Monday, **2017-11-20**.
        - Many of you could do this task **right now** to get ahead of things a bit. Note that this is a **corrected** date.

3. Upcoming non-project Deliverables
    - In a change, [Assignment 5](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-5.md) is now due at noon on Thursday **2017-11-09**. This is delayed six days, so it is now the day after Project Task C is due.
    - Read Silver, through Chapter 11 by 2017-11-02.
    - Quiz 2 will be released on Thursday 2017-11-09 by 5 PM and is due on Monday **2017-11-13** at noon.
        - To help with your review, a brief [additional example on key Part A material](https://github.com/THOMASELOVE/431homework/tree/master/Extra_A) is available. Answer Sketch coming soon.
    - Leek, Chapters 7-8 should be read by 2017-11-14.
    - Silver Chapter 12 by 2017-11-28, and finish the book by 2017-12-05.

4. Some Tips
    - **Use R Projects.** I cannot emphasize enough how important it is to use R Projects in R Studio. Your first step in any analysis should be to create a new Project in a clean directory on your computer, in which you'll store your data, markdown files, etc. I have a separate project for each class, for each homework assignment, for the Course Project. If you're storing everything from the whole course in one place, without any subdirectories, it will be a real challenge if you start having problems. Using [R Projects](https://support.rstudio.com/hc/en-us/articles/200526207-Using-Projects) certainly gets R to default to a sensible choice of directory, which is already a big help. But it has [several other advantages](https://swcarpentry.github.io/r-novice-gapminder/02-project-intro/), too. When you have projects that are more substantial - not just one data set, not just one analysis (as the homework lulls you into developing) using a project will make your life considerably easier.
    - **Visualization "do and don't" advice.** The big advantage of using ggplot2 and the tidyverse more generally is that it's easier to fall into a good plot as long as you tidy your data appropriately. For some advice on visualizing data more effectively, I recommend [this guide by Jenny Bryan](http://stat545.com/block015_graph-dos-donts.html) and its list of resources, which include [these materials from Karl Broman](https://github.com/kbroman/Talk_Graphs). 
    - **Jenny Bryan is a name you want to know.** Incidentally, a good pro tip (from [Michael Lopez on Twitter](https://twitter.com/StatsbyLopez/status/916348419547062272/photo/1)) is that when you're searching for help on using R, add Jenny Bryan at the end. In a crowded universe of advice on programming well, her materials are always outstanding. 
    
## Announcements after class:
