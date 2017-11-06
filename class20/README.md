# Class 20: 2017-11-07

## Today's Slides

Today's Slides are available for download in both [PDF](https://github.com/THOMASELOVE/431slides/blob/master/class_20/431_2017_class-20-slides.pdf) and [R Markdown](https://github.com/THOMASELOVE/431slides/blob/master/class_20/431_2017_class-20-slides.Rmd) formats. 

When the audio recording for today's class becomes available, we'll post it above.

## Announcements before class:

1. Today's Agenda
   - Chi-square testing for 2-way and k-way tables ([Course Notes](https://thomaselove.github.io/431notes/), sections 32-33)
   - Review of material on inference for rates and proportions (Sections 29-31)
   
2. The Projects
     - [Task C](https://github.com/THOMASELOVE/431project/tree/master/TaskC) will be due at noon tomorrow, **2017-11-08**. 
        - The Class Survey is [now available as a Google Form](https://goo.gl/forms/bB1xJ16NnLihP9Gu1) accepting responses.
        - You **also need** to submit [this Word template](https://github.com/THOMASELOVE/431project/blob/master/TaskC/2017_task_C_template_for_YOUR_NAME.docx) via Canvas by noon on 2017-11-08. [A PDF version](https://github.com/THOMASELOVE/431project/blob/master/TaskC/2017_What-does-the-Project-Task-C-template-look-like.pdf) is also available so you can see what is required.
    - [Task D](https://github.com/THOMASELOVE/431project/tree/master/TaskD) is due via email to Dr. Love noon Monday, **2017-11-20**.
        - Many of you could do this task **right now** to get ahead of things a bit. Note that this is a **corrected** date.
        - If you're working with NHANES data, I want to know what tables you used, and I want your cleaned tidied data set, but I don't need the raw pulls.

3. Upcoming non-project Deliverables
    - [Assignment 5](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-5.md) is due at noon on Thursday **2017-11-09**. 
    - (**Note: change in deadline**) Quiz 2 will be released on Thursday 2017-11-09 by 5 PM and will be due on Tuesday **2017-11-14 at 8 AM**. Note that this is change from the original plan (2017-11-13 at noon).
        - The Quiz has 41 questions, and makes use of several **data sets**, which are now available on [our data page](https://github.com/thomaselove/431data).
        - In addition to the Google Form (which is where you **must** take the Quiz) I will also provide access to a password-protected PDF of the Form, so you can look that over offline as you like.
        - Four questions (including Question 1) will likely take you longer than the other 37. Those four questions are clearly marked, and are worth 5 points each. All other items are worth 2, 2.5 or 3 points each, and the Quiz is graded on a scale of 0-120.
        - Essentially everything on the Quiz has been discussed in classes 1-21 or is discussed in Sections 1-33 of the Course Notes.
        - To help you prepare for Quiz 2, 
            - we built a brief [additional example on key Part A material](https://github.com/THOMASELOVE/431homework/tree/master/Extra_A) is available. [Answer Sketch here](https://github.com/THOMASELOVE/431homework/blob/master/Extra_A/extra_A.pdf).
            - You can review many key Part B materials for Quiz 2 in Sections 27 and 36 of the [Course Notes](https://thomaselove.github.io/431notes/index.html) which also contain answer sketches. 
   - [Assignment 6](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-6.md) is due at noon **2017-12-01**.

4. Points of Clarification and Information (reacting to student feedback)
    - If you use `read.csv` to read in a file, then if you want to create a tibble, you need to pipe the result into the `tbl_df` function. If you instead use `read_csv` to read in a file, then it creates a tibble automatically. So why not use `read_csv` all the time? Because it doesn't create factors out of string variables, and, at least in 431-432, that's usually what we want it to do.
    - Working with dates can be tricky. The tidyverse approach uses [the lubridate package](http://lubridate.tidyverse.org/). Take a look, especially if your project data contain dates.
    - Dealing with geographic regions in your project? It's helpful to work with official divisions.
        - Want to identify regions of the United States? The Census Bureau has identified [9 official divisions](https://en.wikipedia.org/wiki/List_of_regions_of_the_United_States#Official_regions_of_the_United_States).
        - Want to sort countries of the world into regions? The UN [categorizes its member states into 5 regions](https://en.wikipedia.org/wiki/United_Nations_Regional_Groups).
        - Want to divide Ohio's 88 counties into regions? I suggest [the approach in this image](http://ohiostockphotography.com/root/OhioStockPhotography/editorAssets/lrg/New%20Ohio%20Regions%20Map%20350dpi%20copy.jpg), although there are many reasonable alternatives.
    - Here's a note on the distinction between [extraversion and extroversion from Scientific American](
https://blogs.scientificamerican.com/beautiful-minds/the-difference-between-extraversion-and-extroversion/
). This comes up because the TIPI (Question 52 on our projecy survey) spells this (appropriately, as it turns out) as "extraversion".
   - You may find the [data.world](https://data.world/) project interesting. I know nothing about it, personally.
   - Some issues (typos, plus some graphs not displaying properly) have been corrected in the [Course Notes](https://thomaselove.github.io/431notes/), sections 26 and 27.

5. The play I am appearing in is "**It's a Wonderful Life**" and it is based on the holiday film directed by Frank Capra, starring Jimmy Stewart and Donna Reed. I play the role of Uncle Billy, at [Independence Community Theatre](http://www.independencetheatre.org/). If you would like to attend or want more information, tickets are available for $12 by calling 216-447-0443. The theater is located at the Old Independence Town Hall, 6652 Brecksville Rd, Independence OH. **PLEASE feel absolutely ZERO obligation to attend**. I mention this so you have the details if you are interested. I would be happy to see you there, but you won't get any extra credit for coming, *nor will I think any less of you should you not attend*.
    - Remaining performances are:
        - at 8 PM on Friday Nov 10, Saturday Nov 11, and 2 PM on Sunday Nov 12.
        - and at 8 PM on Friday Nov 17 and Saturday Nov 18.
   
## Announcements after class:
