# Lead_Score_Case_Study_SB
This assignment is a Logistic-Regression programming assignment wherein I have to build a logistic regression model for the prediction of Hot Leads.

## Table of Contents
* Problem Statement
* Business Goal
* Libraries Used
* Conclusion

## Problem Statement
An education company named X Education sells online courses to industry professionals. On any given day, many professionals who are interested in the courses land on their website and browse for courses. 

The company markets its courses on several websites and search engines like Google. Once these people land on the website, they might browse the courses or fill up a form for the course or watch some videos. When these people fill up a form providing their email address or phone number, they are classified to be a lead. Moreover, the company also gets leads through past referrals. Once these leads are acquired, employees from the sales team start making calls, writing emails, etc. Through this process, some of the leads get converted while most do not. The typical lead conversion rate at X education is around 30%. 

Now, although X Education gets a lot of leads, its lead conversion rate is very poor. For example, if, say, they acquire 100 leads in a day, only about 30 of them are converted. To make this process more efficient, the company wishes to identify the most potential leads, also known as ‘Hot Leads’. If they successfully identify this set of leads, the lead conversion rate should go up as the sales team will now be focusing more on communicating with the potential leads rather than making calls to everyone.

X Education has appointed you to help them select the most promising leads, i.e. the leads that are most likely to convert into paying customers. The company requires you to build a model wherein you need to assign a lead score to each of the leads such that the customers with higher lead score have a higher conversion chance and the customers with lower lead score have a lower conversion chance. The CEO, in particular, has given a ballpark of the target lead conversion rate to be around 80%.

## Business Goal
There are quite a few goals for this case study.

1) Build a logistic regression model to assign a lead score between 0 and 100 to each of the leads which can be used by the company to target potential leads. A higher score would mean that the lead is hot, i.e. is most likely to convert whereas a lower score would mean that the lead is cold and will mostly not get converted.
2) There are some more problems presented by the company which your model should be able to adjust to if the company's requirement changes in the future so you will need to handle these as well. These problems are provided in a separate doc file. Please fill it based on the logistic regression model you got in the first step. Also, make sure you include this in your final PPT where you'll make recommendations.

## Libraries Used
* There are few libraries which are used for the assignment. 
* For analysis and numerical functions, pandas and numpy libraries were imported.
* For Visualization, seaborn and matplotlib libraries were imported
* For Regression, train-test split, RFE, Logistic Regression, adding Constant, VIF, precision score, recall score, etc. were imported from sklearn.
* To avoid warnings, warning's filter was imported.

## Conclusion

* The factors include 'the number of total visits to the website', 'the total time spent on the website', and 'the page views per visit' have the highest impact on the probability of a lead getting converted.

* Lead Source_Welingak Website, Lead Source_Reference, Current_occupation_Working Professional are the top 3 features that contribute positively in getting hot leads.

* The top three variables in my model, that should be focused on are:
   1.  Lead Origin_Landing Page Submission 
   2. Specialization_Others 
   3. Specialization_Hospitality Management
Some specializations have negative impact on leads conversion, even chat conversation impacts negatively.

* Maximum leads as per the data are unemployed as compared to all other occupations.

* Lead Add Form is the only Lead origin where the converted rate is high than nonconverted rate. 

* The difference between Non Converted customers is more than Converted customers, except for Working Professional. Though Working Professional total is not more than 1000 but converted leads percent is higher.

* Customers who do not want to mail them are much less in number as compared to the one who do not want company to email them.

* Lead Source which are Referred have highest lead conversion rates as compared to others which is then followed by Welingak website. Though Google and Other sources have high number of leads generated, their conversion rate is very less.

* Among all the Specializations the leads mostly converted into hot leads is Healthcare Management, but the overall count is very less.
