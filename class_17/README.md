# Class 17: 2017-10-26

## Today's Slides

Today's Slides are available for download in both [PDF](https://github.com/THOMASELOVE/431slides/blob/master/class_17/431_2017_class-17-slides.pdf) and [R Markdown](https://github.com/THOMASELOVE/431slides/blob/master/class_17/431_2017_class-17-slides.Rmd) formats. 

When the audio recording for today's class becomes available, we'll post it above.

## Announcements before class:

1. Today's Agenda
    - The [Course Notes](https://thomaselove.github.io/431notes/) are much larger now, including new Sections 24-35 (finishing Part B) plus some sections of Part C are also in place.
        - We're now recommending that you install the **cowplot** package in R. This is also a good time to update your packages.
    - Power and Sample Size Considerations Comparing 2 Means (see [Course Notes Section 26](https://thomaselove.github.io/431notes/power-and-sample-size-issues-comparing-two-means.html))
        - With `power.t.test` for balanced designs
        - With the `pwr` package for unbalanced designs
    - A little in-class survey
    - Comparing Two Population Means: Decision Support (see [Course Notes Sections 24-25](https://thomaselove.github.io/431notes/comparing-two-means-using-independent-samples.html#a-more-complete-decision-support-tool-comparing-means))
        - The angina example
        - The implant example
    - Developing the Class Survey based on the [Project Task B](https://github.com/THOMASELOVE/431project/blob/master/TaskB/README.md) submissions
    - (if time permits) *The Signal and The Noise*, Chapters 7 and 8
    
2. The Projects
    - Task A: Review the [status of all 43 project proposals](https://github.com/THOMASELOVE/431project/blob/master/TaskA/APPROVED.md).
        - Those of you without an approved proposal (Task A) should be in email contact with me.
    - [Task B materials](https://github.com/THOMASELOVE/431project/blob/master/TaskB/README.md) are due at noon on Monday **2017-10-23**.
        - So far, I've heard from these groups whose Task B looks OK:
            - 4 brains 1 heart (Laura Baldassari, Kedar Mahajan, Sarah Planchon Pope, Sneha Vakamudi, Xin Xin Yu)
            - Shakalaka (Todd Fennimore, Dongze He, Dannielle Skander, Ruipeng Wei, Xueyi Zhang)
            - Club Tukey (Estee Cramer, Chaim Domb, Caroline El Sanadi, Hyung Chul Kim, Vinh Trinh, Frances Wang)
            - The Outliers (Ruke Asagba, Ashlei Beiswinger, Brianna Fuller, Grace Park, Jon Sasse, Pavel Vaisberg)
            - The Foxy Hedgehogs (Sriram Boppana, Laura Cremer, Gavin Hanson, Adam Majot, Arshna Qureshi, Connor Swingle)
        - Two groups submitted Task B on time, but missed part 4, and will, I hope, repair that no later than Thursday at 9 AM:
            - The Two Keys (Jack McDonnell, Neel Patel, Kaylee Sarna, Andrew Tang, Peter Wilkinson)
            - Super 6 (Sophia Cao, Vaishali Deo, J.J. Huang, Preeti Pathak, Andrew Shan, Bilal Zonjy)
        - The other groups didn't have materials on Canvas as of 11 AM, but it's not due until Monday at noon.
            - Pearson Project (Zainab Albar, Abhishek Deshpande, C.W. Gallagher, M.K. Kazimi, Sandra Silva)
            - The Ridiculous Six (Gwen Donley, Sarah Frischmann, Ryan Honomichl, Nik Krieger, Roberto Martinez, Elina Misicka)
    - [Task C](https://github.com/THOMASELOVE/431project/tree/master/TaskC) will be due at noon on Wednesday, **2017-11-08**. 
        - We hope to make the Class Survey available by 2017-10-30.
    - [Task D](https://github.com/THOMASELOVE/431project/tree/master/TaskD) is due via email to Dr. Love noon Monday, **2017-11-13**.
        - Many of you could do this task right now to get ahead of things a bit. **Quiz 2** is also due at that time on that date.

3. Upcoming non-project Deliverables
    - [Assignment 4](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-4.md) is due at noon on Friday **2017-10-27**.
    - [Assignment 5](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-5.md) is due at noon on Friday **2017-11-03**.
    - Quiz 2 will be released on Thursday 2017-11-09 by 5 PM and is due on Monday **2017-11-13** at noon.
