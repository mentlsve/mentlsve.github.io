---
title:  "Basic classification metrics"
date:   2024-09-17 19:31:50 +0000
categories: jekyll update
---


There is a lot of information regarding the confusion matrix and its related metrics on the Internet so I try to avoid repeating it here.
However since I struggeld remembering the most common ones, this is my rewording of it.

When reviewing the literature I think there are 2 different starting points for binary classification problems.

# Tests which are used to confirm a hypothesis or disprove it.

  Classical example would be the medical setting.
  A doctor performs the initial assesssment which leads to a clinical impression (a initial guess). 
  The next step would be to run a test to confirm the clinical impression and if confirmed start with the appropriate treatment.

  I find the following thoughts interesting
  * Running the test on the whole population would result in a very unbalanced dataset, since most people don't have a particular disease. The metric to describe this is called `Prevalence` which is in that the case 

Number of people with disease
-
All people
Number of people with disease + Number of people with disease 


$$
{\color{red} x} + {\color{blue} y}
$$

https://en.wikipedia.org/wiki/Confusion_matrix#Table_of_confusion 

Is this a picture showing a dog or a cat? 
Is this blood sample sadsa.


The picture is showing a cat. True or False.

In all of the above cases we have two possible classes.


We have two classes and they are named `positive`  and `negative` and we have a model which predicts classes for samples.
The model could predict the right class
*  `positive correctly classified as positive` in short a `true positive` 
*  `negative correctly classified as negative` in short a `true negative` 

The model could classify wrongly
*  `positive wrongly classified as negative` in short a `false negative` 
*  `negative wrongly classified as positive` in short a `false positive` 

Accuracy

Recall

true positive / positives