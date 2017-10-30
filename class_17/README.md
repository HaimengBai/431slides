# Class 17: 2017-10-26

## Today's Slides

Today's Slides are available for download in both [PDF](https://github.com/THOMASELOVE/431slides/blob/master/class_17/431_2017_class-17-slides.pdf) and [R Markdown](https://github.com/THOMASELOVE/431slides/blob/master/class_17/431_2017_class-17-slides.Rmd) formats. 

When the audio recording for today's class becomes available, we'll post it above.

## Announcements before class:

1. Today's Agenda
    - The [Course Notes](https://thomaselove.github.io/431notes/) are much larger now, with the addition of 26 new Sections. This includes Sections 24-36 (which finish Part B) plus nearly all of Part C (Sections 37-49). Eventually, we'll have 50 sections, I think.
        - We're now recommending that you install the **cowplot** package in R. This is also a good time to update your packages.
        - If you're looking for class participation credit, hunting and letting Dr. Love know about typos and things that aren't clear to you in the Notes is always welcome.
    - Power and Sample Size Considerations Comparing 2 Means (see [Course Notes Section 26](https://thomaselove.github.io/431notes/power-and-sample-size-issues-comparing-two-means.html))
        - With `power.t.test` for balanced designs
        - With the `pwr` package for unbalanced designs
    - A little in-class survey
    - Comparing Two Population Means: Decision Support (see [Course Notes Sections 24-25](https://thomaselove.github.io/431notes/comparing-two-means-using-independent-samples.html#a-more-complete-decision-support-tool-comparing-means))
        - The angina example
        - The implant example
    - Developing the Class Survey for the Project 
        - Our discussion will flow from [this document, which combines the original submissions with my comments](https://goo.gl/VmU7cx).
        - This work is based on [these original submissions](https://goo.gl/4UZYAH) from the Project Task B Groups.
    - (if time permits) *The Signal and The Noise*, Chapters 7 and 8
    
2. The Projects
    - Task A: Review the [status of all 43 project proposals](https://github.com/THOMASELOVE/431project/blob/master/TaskA/APPROVED.md).
        - I believe everyone is all set now. Don't forget to apply my comments to future tasks, especially Tasks D/E/F.
    - [Task B materials](https://github.com/THOMASELOVE/431project/blob/master/TaskB/README.md) were [submitted by all groups](https://goo.gl/4UZYAH), and [approved and commented on by Dr. Love](https://goo.gl/VmU7cx).
     - [Task C](https://github.com/THOMASELOVE/431project/tree/master/TaskC) will be due at noon on Wednesday, **2017-11-08**. 
        - We hope to make the Class Survey available by 2017-10-30.
    - [Task D](https://github.com/THOMASELOVE/431project/tree/master/TaskD) is due via email to Dr. Love noon Monday, **2017-11-13**.
        - Many of you could do this task **right now** to get ahead of things a bit. **Quiz 2** is also due at that time on that date.

3. Upcoming non-project Deliverables
    - [Assignment 4](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-4.md) is due at noon on Friday **2017-10-27**.
    - [Assignment 5](https://github.com/THOMASELOVE/431homework/blob/master/431-2017_assignment-5.md) is due at noon on Thursday **2017-11-09**.
    - Quiz 2 will be released on Thursday 2017-11-09 by 5 PM and is due on Monday **2017-11-13** at noon.
        - To help with your review, a brief [additional example on key Part A material](https://github.com/THOMASELOVE/431homework/tree/master/Extra_A) is available. Answer Sketch coming soon.

## Announcements after class:

4. The questions from today's in-class survey were as follows. (We'll discuss the results in Class 18.)
- We chose (using a computer) a random number between 0 and 100. Your number is X = 10 (or 65).
    1. Do you think the percentage of countries which are in Africa, among all those in the United Nations, is higher or lower than X?
    2. Give your best estimate of the percentage of countries which are in Africa, among all those in the United Nations.
    3. Provide a point estimate for Dr. Love’s current weight (in pounds.) If you think in kilograms, multiply kg by 2.2 to get pounds.
    4. Now estimate one interval, which you believe has a 50% chance of including Dr. Love’s current weight (again, in pounds.) Then do the same for a 90% interval.

5. The Project Survey draft is [available for your review](https://github.com/THOMASELOVE/431project/blob/master/TaskB/2017-10-27_draft_for_review_81itemsforclassprojectsurvey.pdf). Someone from your Task B group needs to complete [this Google Form](https://docs.google.com/forms/d/1PMVkdEmgIQ1LQWoJL8lOaDAC8gT4PYIIH3Ga3ldZeI4/edit) to share your group's suggested comments or changes before noon on Monday 2017-10-30. Thanks.

6. The [Assignment 4 Answer Sketch](https://github.com/THOMASELOVE/431homework/blob/master/HW4/README.md) is now available in both R Markdown and (password-protected) PDF.
