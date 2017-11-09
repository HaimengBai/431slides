# Class 21: 2017-11-09

## Today's Slides

Today's Slides are available for download in both [PDF](https://github.com/THOMASELOVE/431slides/blob/master/class_21/431_2017_class-21-slides.pdf) and [R Markdown](https://github.com/THOMASELOVE/431slides/blob/master/class_21/431_2017_class-21-slides.Rmd) formats. 

When the audio recording for today's class becomes available, we'll post it above.

## Announcements before class:

0. **VERY IMPORTANT** Tuesday 2017-11-14 11:30 AM - 12:30 PM Office Hours are CANCELLED. Other office hours that day are unaffected. Thank you.

1. Today's Agenda
    - Answering the Airplane Etiquette Exercises posed in Class 20
        - The original [FiveThirtyEight article](https://fivethirtyeight.com/features/airplane-etiquette-recline-seat/) by Walt Hickey.
    - Two "New" Studies worth a little extra look
        - A Double-blind RCT of Stents in Stable Angina
            - [New York Times 2017-11-02](https://www.nytimes.com/2017/11/02/health/heart-disease-stents.html?smprod=nytcore-ipad&smid=nytcore-ipad-share&_r=0) "Unbelievable": Heart Stents Fail to Ease Chest Pain, by Gina Kolata
            - Al-Lamee R et al. Percutaneous coronary intervention in stable angina (ORBITA): a double-blind, randomised controlled trial [The Lancet 2017-11-02](http://www.thelancet.com/journals/lancet/article/PIIS0140-6736(17)32714-9/fulltext?elsca1=tlxpr) 
        - Advil + Tylenol vs. Opiods + Tylenol for acute pain in the emergency room
            - [New York Times 2017-11-08](https://nyti.ms/2hUIj4O) "Alternatives to Opioids for Pain Relief" by Nicholas Bakalar
            - Chang AK et al. Effect of a Single Dose of Oral Opioid and Nonopioid Analgesics on Acute Extremity Pain in the Emergency Department: A Randomized Clinical Trial [JAMA 2017-11-07](https://jamanetwork.com/journals/jama/article-abstract/2661581)
    - Some thoughts on *p* values, statistical significance and *p*-hacking, plus an introduction of two related concepts: **researcher degrees of freedom** and **the garden of forking paths**.
        - The key references are linked in today's slides, also described in detail [in my talk yesterday and its related links](https://github.com/THOMASELOVE/RCR2017).
        - [Andrew Gelman's blog](http://andrewgelman.com/) is how I first heard about much of this material.
        - The **p-hacking** example I'll show is part of [Science isn't broken](https://fivethirtyeight.com/features/science-isnt-broken/#part1) by Christie Aschwanden with graphic by Ritchie King at FiveThirtyEight.com
        - I'll postpone our planned discussion of retrospective design, power, and Type S and Type M errors for a while, in part because an ASA Symposium entitled [Scientific Method for the 21st Century: A World Beyond p < 0.05](https://ww2.amstat.org/meetings/ssi/2017/onlineprogram/Program.cfm) was held last month, and touched on a lot of these issues. I need to find more time to read up on what people were saying there, so I can distill it effectively.

2. Quiz 2
    - A link will appear here after today's class to the Google Form for Quiz 2.
    - A link is coming for a password-protected version of the questions on the Google Form, to facilitate offline work.
    - The data sets you'll need for the Quiz are posted at [our data site](https://github.com/thomaselove/431data).
        - Included are data sets for Q01 (oscar_1 and oscar_2) as well as Q11 (data11), Q19 (data19), Q22 (data22) and Q35 (data35).
        - My answer sketch loads only the forcats and tidyverse packages, but also sources in Love-boost.R, and you'll definitely need Love-boost.R, for the `twobytwo` function, if nothing else.
    - If you have questions, ask them at 431-help.

3. The Projects
     - By now, you've completed Tasks A-C.
        - Actually, as things stand, everyone's completed A, B and the Survey, but one person hasn't finished the Task C Word document. I am still reviewing those materials. We have *n* = 50 respondents to the Survey.
     - [Task D](https://github.com/THOMASELOVE/431project/tree/master/TaskD) is due via email to Dr. Love noon Monday, **2017-11-20**.
        - If you're working with NHANES data, I want to know what tables you used, and I want your cleaned tidied data set, but I don't need the raw pulls.

4. Upcoming non-project Deliverables
    - By now, you've completed Assignment 5. An answer sketch will be posted **today**.
    - [Assignment 6](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-6.md) is due at noon **2017-12-01**.

5. The play I am appearing in is "**It's a Wonderful Life**" and it is based on the holiday film directed by Frank Capra, starring Jimmy Stewart and Donna Reed. I play the role of Uncle Billy, at [Independence Community Theatre](http://www.independencetheatre.org/). If you would like to attend or want more information, tickets are available for $12 by calling 216-447-0443. The theater is located at the Old Independence Town Hall, 6652 Brecksville Rd, Independence OH. **PLEASE feel absolutely ZERO obligation to attend**. I mention this so you have the details if you are interested. I would be happy to see you there, but you won't get any extra credit for coming, *nor will I think any less of you should you not attend*.
    - Remaining performances are:
        - at 8 PM on Friday Nov 10, Saturday Nov 11, and 2 PM on Sunday Nov 12.
        - and at 8 PM on Friday Nov 17 and Saturday Nov 18.

6. Course Notes - edited Section 16 to use Love-boost.R not its precursor.

7. Just for fun, you might want to look at this Tidyverse Case Study by Nick Tierney [Exploring the Billboard Charts](http://www.njtierney.com/post/2017/11/07/tidyverse-billboard/) - although I notice a few of the ggplots aren't showing up yet.

## Announcements after class:

- Good luck on Quiz 2!
