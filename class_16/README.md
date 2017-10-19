# Class 16: 2017-10-19

## Today's Slides

Today's Slides are available for download in both [PDF](https://github.com/THOMASELOVE/431slides/blob/master/class_16/431_2017_class-16-slides.pdf) and [R Markdown](https://github.com/THOMASELOVE/431slides/blob/master/class_16/431_2017_class-16-slides.Rmd) formats. 

When the audio recording for today's class becomes available, we'll post it above.

## Announcements before class:

1. Project Task A Revisions were due at 9 AM today.
  - **13** of the 27 projects that needed a revision have been reviewed on Canvas by Dr. Love so far. 
  - To see your review, visit https://goo.gl/suK7VU or read Dr. Love's comments to you on Canvas.
  - The following revised Task A proposals are **OK/Approved**, in addition to the 17 proposals approved originally. 
    - Abhishek Despande, Gwendolyn Donley, Dongze He, J.J. Huang
    - Grace Park, Neel Patel, Andrew Shan, Frances Wang, Xueyi Zhang
  - Everyone without an approved Task A needs to get another revision in by **Friday 2017-10-20 at 4 PM**.

2. Today's Agenda
  - Comparing Population Means (see [Course Notes](https://thomaselove.github.io/431notes/), especially Chapters 16-22)
  - [Finally, A Formula for Decoding Health News](https://fivethirtyeight.com/features/a-formula-for-decoding-health-news/) from FiveThirtyEight and Jeff Leek.
  - Our opening video comes from [this story at FiveThirtyEight](http://fivethirtyeight.com/features/not-even-scientists-can-easily-explain-p-values/). My favorite part of  the article comes from its close:
      - Try to distill the p-value down to an intuitive concept and it loses all its nuances and complexity, said science journalist Regina Nuzzo, a statistics professor at Gallaudet University. "Then people get it wrong, and this is why statisticians are upset and scientists are confused." **You can get it right, or you can make it intuitive, but it’s all but impossible to do both.**

3. On Artifical Data Codes

- Retraction Watch: [Boys Will Be Boys: Data Error Prompts U-Turn on Study of Sex Differences in School](http://retractionwatch.com/2017/10/17/boys-will-boys-data-error-prompts-u-turn-study-sex-differences-school/)
- [Jessica Logan: "This, my friends, is why you NEVER make a variable called “gender” but instead make one called “male” with responses of 1= yes and 0= no."](https://twitter.com/jarlogan/status/920312287595864064)
- [Jenny Bryan: "Artificial data codes are rarely worth it with modern s/w & h/w. Treated, control, dead, alive, wildtype, mutant … just say it."](https://twitter.com/jennybryan/status/920505719673278465?refsrc=email&s=11)

4. Claudia points out some enjoyable **data art** at http://www.r-graph-gallery.com/portfolio/data-art/
  - For example, consider this look at [BB-8](http://www.r-graph-gallery.com/144-droid-bb-8-data-art/)
  
5. Upcoming Readings/Assignments/Deadlines:
    - **2017-10-23** at noon: [Project Task B](https://github.com/THOMASELOVE/431project/tree/master/TaskB) is due.
    - No class on Tuesday 2017-10-24 (Fall Break.)
    - (delayed to 2017-10-26) Silver Chapters 7 and 8.
    - [Assignment 4](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-4.md) is postponed one week, and will be due on **2017-10-27** at noon.
    
## Announcements after class:

6. On p values
  - The American Statistical Association's [Statement on p-Values: Context, Process and Purpose](http://amstat.tandfonline.com/doi/pdf/10.1080/00031305.2016.1154108)
    - "Informally, a p-value is the probability under a specified statistical model that a statistical summary of the data (e.g., the sample mean difference between two compared groups) would be equal to or more extreme than its observed value."
    - In February 2014, George Cobb, Professor Emeritus of Mathematics and Statistics at Mount Holyoke College, posed these questions to an ASA discussion forum: 
      - Q: *Why do so many colleges and grad schools teach p = 0.05?* 
      - A: Because that’s still what the scientific community and journal editors use. 
      - Q: *Why do so many people still use p = 0.05?* 
      - A: Because that’s what they were taught in college or grad school.
    - "Scientific conclusions and business or policy decisions should not be based only on whether a p-value passes a specific threshold."
    - [XKCD](https://xkcd.com/882/) has a particularly important view to share.
    - Today's video came from "[Not Even Scientists Can Easily Explain P-values](http://fivethirtyeight.com/features/not-even-scientists-can-easily-explain-p-values/)" by Christie Aschwanden at FiveThirtyEight.
    - More from FiveThirtyEight on the ASA's P Values statement in this article: "[Statisticians Found One Thing They Can Agree On: It’s Time To Stop Misusing P-Values](http://fivethirtyeight.com/features/statisticians-found-one-thing-they-can-agree-on-its-time-to-stop-misusing-p-values/)", also by Christie Aschwanden.

7. P Values are a HOT topic.
  - Benjamin et al. 2017 [Redefine statistical significance](https://psyarxiv.com/mky9j/) in which the abstract begins: "We propose to change the default P-value threshold for statistical significance for claims of new discoveries from 0.05 to 0.005." 
    - [Article in Science Magazine online](http://www.sciencemag.org/news/2017/07/it-will-be-much-harder-call-new-findings-significant-if-team-gets-its-way) about the Benjamin et al. piece 
    - [Gelman](http://andrewgelman.com/2017/10/02/response-comments-abandon-statistical-significance/) comments: Benjamin et al. recommend replacing 0.05 by 0.005, not because they think a significance-testing-based lexicographic decision rule is a good idea, but, as I understand them, because they think that 0.005 is a stringent enough cutoff that it will essentially break the current system. Assuming there is a move to reduce uncorrected researcher degrees of freedom and forking paths, it will become very difficult for researchers to reach the 0.005 threshold with noisy, useless studies. Thus, the new threshold, if applied well, will suddenly cause the stream of easy papers to dry up.
  - Amrhein and Greenland Letter to the Editor, "[Remove, rather than redefine, statistical significance.](https://www.nature.com/articles/s41562-017-0224-0.epdf?author_access_token=L959flsJ2VSamUFJCWIOzNRgN0jAjWel9jnR3ZoTv0MAP1jqVPztYsCvh9lHmAlkugywnGK1u0jOW2TvCE7rKZ06gNuva193la619LstweNrBRHEw8Fcq3oOwSqNdeaQrEUugNqJsU8THmLMIZiPFg%3D%3D)"
  - McShane, Gal, Gelman, Robert and Tackett 2017 **Abandon Statistical Significance**. Here's [the blog post](http://andrewgelman.com/2017/09/26/abandon-statistical-significance/) and [the full paper](http://www.stat.columbia.edu/~gelman/research/unpublished/abandon.pdf) 
  - Lakens et al. [Justify Your Alpha](https://psyarxiv.com/9s3y6) - "In response to recommendations to redefine statistical significance to p <= .005, we propose that researchers should transparently report and justify all choices they make when designing a study, including the alpha level."
  - [Should We Redefine Statistical Significance? A Roundtable at Brains Blog](http://philosophyofbrains.com/2017/10/02/should-we-redefine-statistical-significance-a-brains-blog-roundtable.aspx)
  - [Gelman](http://andrewgelman.com/2017/10/10/please-contribute-list-top-10-dos-donts-better-science/) again: "Measurement error and variation are concerns even if your estimate is more than 2 standard errors from zero. Indeed, if variation or measurement error are high, then you learn almost nothing from an estimate even if it happens to be 'statistically significant.'"
  - We'll have more to say about p hacking and the garden of forking paths down the line.
  - So what can be done?
    - zbicyclist, [here](http://andrewgelman.com/2017/10/10/please-contribute-list-top-10-dos-donts-better-science/#comments), comments: "Learn from the data mining people. They know they are going to go down the garden of forking paths, and so split the data into a Training set and a Test set (sure, 10-fold cross-validation is cooler, but let’s not get ahead of ourselves here)."
    - (Gelman and Hill) "We have essentially no interest in using hypothesis tests for regression because we almost never encounter problems where it would make sense to think of coefficients as being exactly zero. Thus, rejection of null hypotheses is irrelevant, since this just amounts to rejecting something we never took seriously in the first place. In the real world, with enough data, any hypothesis can be rejected. That said, uncertainty in estimation is real, and we do respect the deeper issue being addressed by hypothesis testing, which is assessing when an estimate is overwhelmed by noise, so that some particular coefficient or set of coefficients could just as well be zero, as far as the data are concerned. We recommend addressing such issues by looking at standard errors as well as parameter estimates."
