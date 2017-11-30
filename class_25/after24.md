# Feedback from the "Activity After Class 24"

44 people completed the activity in a timely fashion, of whom 40 actually attended the class.

## Project Titles

Some people have weak titles. Titles on graphs and subtitles within an analysis are amazingly important.

I saw three types of common problems. 
- **Filler**. You've included words that add nothing like "A Study of" or "The Impact of" "Effect of" or "The association of", etc.
- **Grammar/Syntax**. A title, though an abbreviated statement and rarely a sentence, still should conform to standard English as much as possible. Spell things correctly - use proper tenses, etc. If English isn't your first language (and even if it is), cultivate a reader who can look at a title or an abstract for you and make useful edits.
- **Too much detective work required** Your title, ideally, will address Who was studied, How and Why they were studied and What the results were, all in 15 words or less. The best strategy is often to answer most (if not all) of these questions in a declarative sentence, then prune out anything that isn't vital.
    
Two titles I happened to like follow. 
- Can wealth help save Sudanese daughters from female genital mutilation? 
- Unpacking the Relationship between Insurance Coverage and Alcohol Consumption

There were others I could have chosen, and a title's never perfect, but they illustrate some good things.

## The Top Ten "Most important things learned in Class 24" 

1. **Graphs** are a vital part of my Project presentation (Task F) as well as my paper (Task E).
2. Interpreting the regression equation in **words** is the hard part.
3. **Significance Testing in a Model**. Interpreting ANOVA and t tests for a regression model. "Last predictor in" interpretation of t tests and when the order of predictors matters (ANOVA) and doesn't matter (t tests)
4. **Collinearity**. The true predictive value of a predictor may be masked by another predictor if they are strongly correlated with each other
5. **R^2^ and Adjusted R^2^**. The multiple R-square is greedy - it will always look better when you add more variables, but that does not necessarily mean that your model is better. The adjusted R^2^ trades off predictive power and the number of predictors in the model. If the R^2^ and adjusted R^2^ are similar, then the predictive power the R^2^ implies is more likely to hold up in predicting new data using the model. If adjusted R^2^ is much smaller than R^2^, then the model probably includes some predictors that could be omitted.
6. **Box-Cox plot**. This is a tool to help guide us to useful transformations of a quantitative outcome to deal with violations of the assumptions of linearity. Oh, and Box-Cox (and the transformations it assesses) expects the outcome to be strictly positive - no zeros and no negative values.
7. **Residual Plots**. What we're looking for, and what we do about it if we find it (a curve in the residual vs. fitted plot, for instance, to indicate non-linearity)
8. **Residuals, Leverage and Influence**. Assessing whether an outlying point is influential on the model via Cook's distance.
9. **Building a scatterplot matrix**. Enter the outcome variable *last* in `GGally::ggpairs` when building a scatterplot matrix.
10. **Comparing Models**. Comparing AIC, BIC, or R^2^ values between models is only meaningful if we are predicting the same outcome in each model. If one predicts Y and the other predicts log Y, then the decision about which model is best shouldn't rely on these sorts of summaries.

## The Top Six "Muddiest" Things That People Were Thinking About After Class 24

1. **Variable Selection**, both in terms of potential *collinearity* (if we have two predictors that are strongly correlated with each other, for example, how do we select a model that includes one or the other?) and more generally (how do we prune a large model sensibly?)
2. **Which R^2^**. R^2^ vs. Adjusted R^2^ - which should we use, and when?
3. **Transforming the Outcome**. What are the good choices, what should we take into consideration in selecting to transform or not transform, and if we predict, say, log(Y) instead of Y, how do we back transform our predictions at the end? And also, do we sometimes transform the predictors instead of the outcome?
4. **Ordering the Predictors**. Does it matter what order we put the predictors into the model? Does the order change what equation is fit? Does it change what the t tests indicate? Does it change what the ANOVA tests indicate? And what if we have a multi-categorical predictor - does it matter what we choose as the baseline category, and what is specified by the indicator (dummy) variables?
5. **Residuals, Leverage and Influence**. How should we interpret this plot? What do we do if we have points with high leverage but not high influence, and what should we do if we have points with high influence?
6. **VIF** - what is the variance inflation factor and how should we think about collinearity generally?
