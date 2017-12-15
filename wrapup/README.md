# End of Semester Wrap Up page

This is the place for all of Dr. Love's communications after our final class.

## For everyone who's completed the project, a course grade is now available.

[See this link](https://github.com/THOMASELOVE/431slides/blob/master/wrapup/GRADES.md) for more details. 

- You should receive an email from Professor Love before 2017-12-16 outlining your scores.

## Quiz 3 Grades are Complete

- **NEW!** The answer sketch is now posted above, and you'll receive an email with your grade at your CWRU account (I sent them at 10 AM on Thursday 2017-12-14) and that email will let you see how you did on each question and overall.

## Appealing Homework Grades

I received Google Form requests to appeal homework grades from five people, all of whom have heard back from me via email.

## Course Evaluation for The University

You have received [emails from the University about their evaluation of the course](https://webapps.case.edu/courseevals/). As I understand it, those of you enrolled in PQHS 431 may not have been receiving those emails, but you should now be getting them. At any rate, [visit this link](https://webapps.case.edu/courseevals/) to complete that eveluation by the deadline of 2017-12-21.

## Course Evaluation for me

In addition to the University evaluation, I would be **extremely** grateful if you completed [this evaluation](https://goo.gl/forms/DD2hL8g6GOHxCzwc2) for me as soon as you can. As of 2017-12-14 at 10:35 PM, I had received this from 45/50 people, so thank you very much!

## Christmas Wassail Concert

Dr. Love is one of five featured singers in the annual Wassail Christmas Concert given by the Chagrin Studio Orchestra at Chagrin Valley Little Theater on December 22 and 23 starting at 6:15 (wassail and cookies), 7:00 (downbeat) each evening. Wrap yourself up in the music of the season with 40+ of Cleveland's finest musicians for a mere $25 (adults) and $15 (students). If you are interested, visit [CVLT's Tickets page](https://app.arts-people.com/index.php?show=81251). It is my understanding that the concerts will sell out in advance.

## Preparing for 432

Those of you taking 432, thank you for your interest.

- The course begins January 16, and I cannot promise to have anything ready for you before that date. If I do, I'll let you know here.
- Dr. Love will be at CWRU on 2017-12-21. If you need to talk to him, send an email. He will be away from email Dec 23 - Jan 2 and again from Jan 7 - 14.
- 431-help is now closed. We'll reopen on the first day of 432 class: 2018-01-16. We still call it 431-help in 432.
- If you want to see a list of potential topics for 432 and some indication of likely emphasis, [click here](https://github.com/THOMASELOVE/431slides/blob/master/class_27/taskafter26.md) and scroll down. I've linked a few things there.
    - I'll encourage you to continue working with R, and a very useful thing to do is read [R for Data Science](http://r4ds.had.co.nz/) and work on some of the trickier materials there.
    - I'll also encourage you to look at Jenny Bryan's [Happy Git with R](http://happygitwithr.com/), and be sure to email me your GitHub account name.
    - It can't hurt to review R Studio's [extensive and growing list of webinars](https://www.rstudio.com/resources/webinars/) designed to help you get more out of your R and R Studio experiences. This is a great place to get started learning about, for example, Shiny.

## Project Hints / Suggestions

I have placed a PDF copy of the [form I will use to evaluate Fall 2017 Project Presentations here](https://github.com/THOMASELOVE/431project/blob/master/TaskF/TaskF_evaluationformforTELtouse_(Mondayversion).pdf) for you to review, if you are interested. This is a form for me, not you, but it may help you to see what is on the form.

1. **Don't fit impossible kitchen sink models.** When fitting a kitchen sink model, count the number of observations in your training data set. Call that N. Then count the number of coefficients (slopes + intercept) you are planning to fit. Call that COEFFS. If N / COEFFS < 15, then you should be reducing the number of coefficients you are trying to fit in your kitchen sink model. If N / COEFFS < 10 or so, then this becomes absolutely imperative. Ideally, N / COEFFS should be 20 or more for a straightforward kitchen sink model.
2. **If you can, include a meaningful name as a variable in your data.** For example, if your rows describe countries, have a variable called "Country" - even though you will not use this as a predictor, it's very helpful for identifying outliers, etc.
3. **Pretty Code** Put a blank line before and after each code chunk. Put a blank line before and after each heading (and use lots of headings and subheadings) to help you find things when you present your results.
4. **Check your list of packages** Make sure `library(tidyverse)` is your last loaded library, and that you don't include any packages you don't actually need to include. 
    - In particular, if you have `library(tidyverse)` in your code, that means you have loaded eight packages now: `ggplot2`, `dplyr`, `tibble`, `readr`, `purrr`, `tidyr`, `stringr` and `forcats`. So you don't need to load any of those eight beforehand.
    - Also, if you are going to write `mosaic::favstats` every time you want to use `favstats` and you're not using any other functions from the `mosaic` package, then don't include `library(mosaic)`.
    - Similarly, don't include `library(Hmisc)` if the only function you will use from `Hmisc` is `describe`, and every time you plan to call it, you'll use `Hmisc::describe`.
5. **Don't use pander with the results of a by function**: It won't work, even though I did it in one of the demonstrations. Just drop the `pander` piece.
6. **What do I do with this association plot in Study 1?** At the bottom of page 44 of the study 1 demonstration pdf, I describe the plot that is produced on that page. I suggest you follow that model to analyze your plot. The plot shows the size of the residuals for the model of independence. Large boxes indicate bigger deviations from independence than smaller boxes. Boxes above the horizontal line indicate positive residuals, boxes below the horizontal line indicate negative residuals. The width of each boxes indicates how many observations fall in that combination of categories on the contingency table, and the height indicates the size of the residual for that combination of categories on the contingency table.
7. **Can I use Powerpoint to present in Task F, or should I just use the HTML files I generated for Task E?** It's entirely up to you.
8. **If you've given multiple ways (say, (a) and (b)), to accomplish the same thing, should I use method (a) or method (b)?** Your choice.
9. **Should everyone be using exactly the same Excel data sets and setup code Dr. Love provided to set up the Study 1 (class survey) data?** Yes.
10. **What about back-transformation if I fit a model with, say, the log of my original outcome?** In Study 2, you may wind up transforming your outcome. If you use, for example, a log transformation, then everything in your training sample should be done on the log scale. But when you predict into your **test** sample, make the predictions of the log(outcome) and then exponentiate them to get them back on the original outcome scale before you calculate prediction errors and then form MSPE and MAPE and Mean Absolute Error.

Oh, and Jenny Bryan wrote a great article about Projects and Workflow that we'll discuss in 432. [Take a look](https://www.tidyverse.org/articles/2017/12/workflow-vs-script/).

# Old Stuff that used to be on this page

A. This week, you need to:

1. Submit **Quiz 3** by Tuesday at noon using [this Google Form](https://goo.gl/forms/yj5YuBusGF7hVvnx1).
2. Submit Project [Task E](https://github.com/THOMASELOVE/431project/tree/master/TaskE) by Wednesday at noon via Canvas
3. Submit any **homework grading revision requests** by Wednesday at noon using [the Google Form provided](https://goo.gl/forms/v5zBIuGnrLkbiuXU2) (Assignment 6 [grades are available here](https://github.com/THOMASELOVE/431homework/blob/master/HW6/431-grades6-pw-2017.pdf) - remember that the PDF file is just password-protected.)
4. Give your **presentation** ([Task F](https://github.com/THOMASELOVE/431project/tree/master/TaskF)) on Monday, Tuesday or Thursday according to [the schedule](https://github.com/THOMASELOVE/431project/blob/master/TaskF/SCHEDULE.md).
5. Submit a **course evaluation** (probably after your presentation is best) using [the Google Form I provided](https://goo.gl/forms/DD2hL8g6GOHxCzwc2).
    
B. I built a form ([here is the PDF version for Monday](https://github.com/THOMASELOVE/431project/blob/master/TaskF/TaskF_evaluationformforTELtouse_(Mondayversion).pdf)) that I will use to evaluate your project presentations. If you want to see it, you are welcome to take a look. Remember that this is a form for me to fill out, not you. 

C. There is also a set of 10 or so last minute Project Tips/Hints on the [Wrapup README page](https://github.com/THOMASELOVE/431slides/blob/master/wrapup/README.md) which I hope you will read.

D. 431-help will close on Thursday 2017-12-14 after the final project presentation, but I am sure I will be reviewing questions at the following times (and NOT at most other times). 431-help reopens on 2018-01-16.


E. Quiz 3 stuff
- The [PDF of the questions and response options for Quiz 3 is here](https://github.com/THOMASELOVE/431slides/blob/master/wrapup/431-quiz3-2017.pdf).
    - Correction 1 made 2017-12-07 at 9 PM: In Q32, there are four models, not five.
    - Correction 2 made 2017-12-07 at 9:30 PM: In Q11, the outcome is the log of a measure of predatory behavior, not of diastolic BP.
    - Correction 3 made 2017-12-08 at 11:50 AM: In the setup for Q34-40, I had left out `a1c` as one of the variables. It was always in the data set, and in the actual questions, but was inadvertently left out of the setup materials.
    - Correction 4 made 2017-12-11 at 3:20 PM: In Q07, the data displayed are now correctly labeled as Before - After, not After - Before, so that positive values indicate weight loss, and negative indicate weight gain. 
- The [Google Form](https://goo.gl/forms/yj5YuBusGF7hVvnx1) you'll use to submit your answers to Quiz 3 [is now available](https://goo.gl/forms/yj5YuBusGF7hVvnx1). Remember that you must complete the Quiz by 2017-12-12 at 12 NOON.
- The data and code you'll need for Quiz 3 are posted above, and on [our data page](https://github.com/thomaselove/431data). There are three files, in particular, and they are `hospsim.csv`, `surveyday1_2017.csv` and `wc_code.R`.
- Good luck! 


- Sunday sometime between 7 and 9 PM
- Monday morning before 7:30 AM and then during the day, occasionally, but not after about 4 PM
- Tuesday morning before 8 AM, and then during the day, occasionally, but not after about 5 PM
- Wednesday morning before 9 AM, and again in the evening


5. **Appealing HW Grades**: If you want me to regrade an assignment, review the [Grade Appeal Policy](https://thomaselove.github.io/431syllabus/general-course-policies.html#grade-appeal-policy---wait-until-december) in the Syllabus, and then request a regrade by filling out [this Google Form](https://goo.gl/forms/v5zBIuGnrLkbiuXU2) before noon on Wednesday **2017-12-13**. Grades on Assignment 6 will be made available to you as soon as possible.

1. Good luck on the Quiz and your Project!

2. Getting Help after Dec 8
    - If you are having trouble with R, and asking for help at 431-help, we need to first replicate your problem in order to solve it. So, **PLEASE**:
        1. Send your **entire** R Markdown file. All of it. Not pieces of it. All of it.
        2. Send a **screenshot** of the error message you are receiving, AND specify the line number where things break down if you can in your email. Or ask a specific and detailed question - as specific and detailed as you can make it.
        3. If this is about "your data" **send the data** set(s) that your R Markdown calls. If this is about the class survey data, we have that. But we don't have your data.
        4. Please don't wait until you've been struggling with a problem so long that you feel frustrated or feel the need to tell us how long that's been to garner our sympathy. Struggle for 15 minutes with the demonstration files, then Google or search the course notes for at most another 15 minutes, then email us, is a reasonable workflow. Coding is hard enough with help.
        5. **Don't wait** until the last day. I warn you that I am thoroughly unavailable on Mon 12-11 and Tue 12-12 except for a little bit of time between projects. In particular, I am booked both of those evenings.
