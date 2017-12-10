# End of Semester Wrap Up page

This is the place for all of Dr. Love's communications after our final class.

## Quiz 3: Deadline is Tuesday 2017-12-12 at 12 NOON

- The [PDF of the questions and response options for Quiz 3 is here](https://github.com/THOMASELOVE/431slides/blob/master/wrapup/431-quiz3-2017.pdf).
    - Correction 1 made 2017-12-07 at 9 PM: In Q32, there are four models, not five.
    - Correction 2 made 2017-12-07 at 9:30 PM: In Q11, the outcome is the log of a measure of predatory behavior, not of diastolic BP.
    - Correction 3 made 2017-12-08 at 11:50 AM: In the setup for Q34-40, I had left out `a1c` as one of the variables. It was always in the data set, and in the actual questions, but was inadvertently left out of the setup materials.
- The [Google Form](https://goo.gl/forms/yj5YuBusGF7hVvnx1) you'll use to submit your answers to Quiz 3 [is now available](https://goo.gl/forms/yj5YuBusGF7hVvnx1). Remember that you must complete the Quiz by 2017-12-12 at 12 NOON.
- The data and code you'll need for Quiz 3 are posted above, and on [our data page](https://github.com/thomaselove/431data). There are three files, in particular, and they are `hospsim.csv`, `surveyday1_2017.csv` and `wc_code.R`.
- Good luck! 
    - *Note*: After the deadline passes, a detailed answer sketch will be posted here, and you'll receive an email with your grade at your CWRU account when I've reviewed your work, and this will let you see how you did on each question and overall.

## Project Hints / Suggestions

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


## Announcements

1. Good luck on the Quiz and your Project!

2. Getting Help after Dec 8
    - If you are having trouble with R, and asking for help at 431-help, we need to first replicate your problem in order to solve it. So, **PLEASE**:
        1. Send your **entire** R Markdown file. All of it. Not pieces of it. All of it.
        2. Send a **screenshot** of the error message you are receiving, AND specify the line number where things break down if you can in your email. Or ask a specific and detailed question - as specific and detailed as you can make it.
        3. If this is about "your data" **send the data** set(s) that your R Markdown calls. If this is about the class survey data, we have that. But we don't have your data.
        4. Please don't wait until you've been struggling with a problem so long that you feel frustrated or feel the need to tell us how long that's been to garner our sympathy. Struggle for 15 minutes with the demonstration files, then Google or search the course notes for at most another 15 minutes, then email us, is a reasonable workflow. Coding is hard enough with help.
        5. **Don't wait** until the last day. I warn you that I am thoroughly unavailable on Mon 12-11 and Tue 12-12 except for a little bit of time between projects. In particular, I am booked both of those evenings.

3. I will be one of five featured singers in the annual Wassail Christmas Concert given by the Chagrin Studio Orchestra on December 22 and 23 starting at 6:15 (wassail and cookies), 7:00 (downbeat) each evening. Wrap yourself up in the music of the season with 40+ of Cleveland's finest musicians for a mere $25 (adults) and $15 (students). If you are interested, visit [CVLT's Tickets page](https://app.arts-people.com/index.php?show=81251). 

4. **Course Evaluations** In addition to the University evaluation, I would be extremely grateful if you completed [this evaluation](https://goo.gl/forms/DD2hL8g6GOHxCzwc2) for me as soon as you can. One question refers to the project presentation, but otherwise, you should be able to complete this now. Thank you in advance.

5. **Appealing HW Grades**: If you want me to regrade an assignment, review the [Grade Appeal Policy](https://thomaselove.github.io/431syllabus/general-course-policies.html#grade-appeal-policy---wait-until-december) in the Syllabus, and then request a regrade by filling out [this Google Form](https://goo.gl/forms/v5zBIuGnrLkbiuXU2) before noon on Wednesday **2017-12-13**. Grades on Assignment 6 will be made available to you as soon as possible.

6. **Corrections to the Course Notes**
    - On 2017-12-08 I corrected a small error in Section 30.6, where I had in one place written "relative risk" in the section defining risk difference.
    - On 2017-12-09 I fixed typos in Sections 11 and 30.

6. **432** 
    - Want to get a leg up on 432? I cannot promise I'll have anything ready for you before January 18, I'm afraid. 
    - If you want to see a list of potential topics for 432 and some indication of likely emphasis, [click here](https://github.com/THOMASELOVE/431slides/blob/master/class_27/taskafter26.md) and scroll down. I've linked a few things there.
    - I'll encourage you to continue working with R, and a very useful thing to do is read [R for Data Science](http://r4ds.had.co.nz/) and work on some of the trickier materials there.
    - I'll also encourage you to look at Jenny Bryan's [Happy Git with R](http://happygitwithr.com/), and be sure to email me your GitHub account name.
    - It can't hurt to review R Studio's [extensive and growing list of webinars](https://www.rstudio.com/resources/webinars/) designed to help you get more out of your R and R Studio experiences. This is a great place to get started learning about, for example, Shiny.
