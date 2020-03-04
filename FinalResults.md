# BA 545 Course Project 1: Advanced Preparation of Financial Data
# Team: DeadlineDemons

### Research Question
The overarching research question is “What are the determinants of IPO underpricing phenomena?” In this competition, your main purpose is to prepare the data for predictive models answering the overarching research question.

- After cleaning and modeling the data in various ways, we have determined the best model to be pipeline 2. This pipeline first uses interquartile ratio, then scales the data on a MinMax Scaler, and finally normalizes the data to reduce skewness. Through feature selection we were able to rank the variables according to their impact on the target variables. After running these features through the evaluation code, the best result were seen in pipeline 2, the results are as follows:
    Y1:
        Predictors: Percent of long sentences, Percent of long words, Percent of positive words, Percent                     of negative words.
        F1 score: .6373
    Y2:
        Predictors: Prior Nasdaq 15-day returns, percent of negative words, Share overhang, Up revision,                     Sales.
        F1 score: .6504
- As seen in the results, both F1 scores are above .6, which is a good result. All of our pipeline's evaluation codes resulted in a F1 score of .6 or above. Of all 4 evaluations, pipeline 2 had the highest F1 score for both Y1 and Y2, determining it to be the best model.
    
### Data Dictionary
See attached ‘Data Dictionary’ document ('DataDictionary20190115.pdf').

### Pipelines
The different final pipelines are stored as '*Pipeline1.ipynb', '*Pipeline2.ipynb', '*Pipeline3.1.ipynb', and '*Pipeline3.2.ipynb'. 

Pipeline 2 had the best results.

### Evaluation Code
The evaluation codes we used are stored as 'Pipe1EvalCode.ipynb', 'Pipe2EvalCode.ipynb', 'Pipe3-1EvalCode.ipynb', and 'Pipe3-2EvalCode.ipynb'.

### Processed Data
We have saved the resulting processed data from each of our pipelines as 'pipeline1.csv', 'pipeline2.csv', 'pipeline3_1.csv', 'pipeline3_2.csv'. We used these csv files for feature selection 
and evaluation codes.
