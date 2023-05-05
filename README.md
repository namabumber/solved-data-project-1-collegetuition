Download Link: https://assignmentchef.com/product/solved-data-project-1-collegetuition
<br>
<span class="kksr-muted">Rate this product</span>




You work as a researcher at the US Dept. of Education and are requested to create a predictivemodelofcollegetuitionbasedonanumberofcharacteristics gatheredfrom higher education institutions. The data collected from a sample of US Colleges has 1121 records and includes the following variables:

<ul>

 <li>tuition: College tuition (“out-of-state” rate for those with in-state discount).</li>

 <li>pcttop25: Percent of new students from the top 25% of high school class.</li>

 <li>sf_ratio: Student to faculty ratio.</li>

</ul>

<ul>

 <li>accrate:</li>

 <li>graduat:</li>

 <li>pct_phd:</li>

 <li>fulltime: Percent of undergraduates who are full time students.</li>

 <li>alumni: Percent of alumni who donate.</li>

</ul>

Fraction of applicants accepted for admission. Percent of students who graduate.

Percent of faculty with Ph.D.’s.

<ul>

 <li>num_enrl: Number of new students enrolled.</li>

 <li>public_private: Is the college a public or private institution? public=0, private=1</li>

 <li>fac_comp: Average faculty compensation.The dataset is provided as a CSV file (hint: use the Var source node to read the file)</li>

</ul>

<ol>

 <li>Explore the data to get some initial insights, if you think it is useful (your call)</li>

 <li>Identify outliers and decide what to do with them</li>

 <li>Missing data appears to be a problem with this data set. Prepare a copy of the data set, where the missing values are each replaced with their field means. Report on how this substitution has affected the fields (summary stats, etc.), if at all. What do you think of this method of dealing with missing values?</li>

</ol>

Use the dataset with missing data (not replaced) for items 4 to 6.

4. Provide a table describing the relationship of each explanatory variable with tuition (hint: use scatter plots). If the relationship is not linear, you can1 make it so by transforming the predictor variable. Note: we did not cover this but I’m trying to make you be creative. For example, after looking at the scatter plot, you may find that Y does not have a linear relationship with X1, but you can make it linear by transforming X1(squaring X1 or taking the logarithm). How would you know this? Trial and error. For example square X1 and see how the scatterplot of Y and (X1)^2 looks like. Assuming you make your transformation (e.g. you squared X1), the new variable will be (X1trans), and the regression model will have the functional form, Y=b0+b1*X1trans+b2*X2+…+bk*Xk. This is still a linear regression as we have a linear combination of predictors. The only difference is that you have transformed some variables to improve the fit of your model.

1 Notstrictlyrequired,butmayhelpenhanceyourmodel.Youdecide.

<ol start="5">

 <li>Investigate the correlation among the predictor variables. Suggest a creative course of action (rather than simply omitting a variable) for dealing with any medium or strongcorrelationsencountered(e.g.textbook,section9.7;avoidanymethod linked to principal component analysis, as we have not covered it yet).</li>

 <li>Use SPSS Modeler linear regression tool to investigate whether a linear relationship exists between tuition and the other variables. Investigate the differences in the models,ifany,amongthesemethods:enter,stepwise,backwards. Constructatable showing method, variables included, statistical tests on regression coefficients, goodness of fit metric(s), predictive accuracy metric on training and test data. Discuss. Whichmodeldoyoupreferandwhy?</li>

 <li>Use SPSS Modeler linear regression tool on the data set where the missing values are each replaced with their field means. Investigate the differences in the models, if any, among these methods: enter, stepwise, backwards. Construct a table showing method, variables included, statistical tests on regression coefficients, goodness of f it metric(s), predictive accuracy metric on training and test data. Discuss. Which model do you prefer and why?</li>

 <li>Compare the best model in 6 and the best model in 7. Which model do you prefer and why?</li>

 <li>For the final (chosen) model:a. Write out the estimated regression equation and explain the meaning of the coefficientsb. Provide a full report of the chosen regression model and report its metrics (goodness of fit, predictive performance) and statistics on training and test data</li>

</ol>

Make sure you tweak your models to get the best performance. Use 70/30 partition in all cases

10. Decisiontreeclassification:Usingthepublic_privatevariableascategorical(flag),or deriving from it a flag variable, model the profile of a typical public and private college with a C5.0 decision tree algorithm, using all other variables as predictors (disregard tuition, given the typical difference in tuition between state and private institutions). Compute the confusion matrix and derive proper performance metrics.