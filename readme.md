# Project: Churn Prediction in Massive Open Online Course Enrollment

Summary: Using multivariable logistic regression, I created 3 models to determine the likelihood for churn by MOOC students, a group known for their well-documented lack of commitment to educational products.

# Why I built this project:

Tackle a pervasive business problem: Churn

Demonstrate proficiency in building ML models

Show ability to interpret and present model results

# Techology used: 

Python

# Datasets: Kaggle

https://www.kaggle.com/datasets/imuhammad/edx-courses

https://www.kaggle.com/datasets/edx/course-study

https://github.com/kanika-narang/MOOC_Data_Analysis/blob/master/DATA/cleaned%20data/big_student_clear_third_version.csv

https://www.kaggle.com/datasets/alperkulunkoglu/udemy-courses-2011-2017?select=WebDevelopment.csv

## Model 1- Comprehensice Model

The first model combines demographic, behavioral and content features to predict the likelihood of a student completing a course

Accuracy: 0.9778987116836961

Precision: 0.7510775862068966

Recall: 0.5829383886255924


## Model 2 - Behavioral Model

The second model combines information related to behavior such as the course content accessed and frequency of posting in a discussion forum to predict whether or not a student will pay for an honor code certificate.

Accuracy: 0.999929324340697

Precision 0.9444444444444444

Recall 0.9272727272727272

## Section 4: Model 3 - Content-Based Model

The final model assessed the impact of content attributes such as the number of chapters or number of reviews on a student's decision to view module content.

Accuracy: 0.9567464965066032

Precision: 0.9921654464487886

# Results

For a 75-25 split the multivariable models were very precise, with an accuracy that ranged between 95 and 99 percent. The first model was the weakest out of the three. While its accuracy rate was 97 percent, the model’s precision and recall statistics were considerably lower, at 75 and 60 percent respectively. While a 97 percent accuracy sounds ideal, it is difficult to say, with absolute certainty, that this model is that accurate because the precision and recall rates mean that it did not reliably discern between true positives, true negatives, false positives and false negatives over 75 percent of the time.

The next model reduced the number of independent variables by more than half to six. This time, the model combined hours of certification, course content accessed, percentage audited, the history of a student posting in a discussion forum, the number of students with a bachelor’s degree or higher and a grade higher than zero to predict whether they would earn an honor code certificate and, ultimately, pay for such a distinction (as opposed to conducting a free audit). The reduction of variables resulted in a far more reliable model with an accuracy rate of 96 percent, a precision of 99 percent, and a recall of 95 percent.

The final model combined the least amount of variables, ingesting only four columns: number of chapters, number of events, number of reviews and number of subscriptions to predict how many students would view at least one module. Like the previous model, this combination of a few highly positively correlated variables yielded a high accuracy rate of 95 percent, but more importantly, a precision rate of 99 percent, and a recall rate of 95 percent. However, this model could better discern between actual and predicted labels than the previous two iterations.
Recall: 0.9458203220560936

# Key insights:

Despite a 90% accuracy, the model precision was considerably lower (high 60%)

Best predictors of likelihood to churn included: Percentage of course complete, percentage of course audited and whether or not the individual held a bachelor’s degree

Reduction of features created a more precise model, with accuracy and precision metrics hovering around 95%
