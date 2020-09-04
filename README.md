# Google-Quest-Q-A
Computers are good at answering questions with single verifiable answers. For Example, querying “Who is the Prime Minister of India?” on google, will give a perfect answer. When it comes to answering subjective aspects of a question, Humans do a much better job than what computers do. Few subjective aspects include 
 * Is the question understandable?
 * Is the question conversational?
 * Is the answer to the question understandable?

The CrowdSource team at Google Research, has collected data on a number of these subjective aspects for each question-answer pair.
Crowdsource gathers your feedback, and feedback from others around the world, which helps the machine to learn from accurate examples and improves the services provided by google like Maps, Translate etc. 
The question-answer pairs were gathered from nearly 70 different websites. The raters received minimal guidance and training, and relied largely on their intelligence to answer subjective aspects of the prompts. As such, each prompt was simplified in such a way so that raters could simply use their common-sense to complete the task.
The task here is to build a predictive algorithm which would quantify these subjective aspects given a question-answer pair.
The Evaluation Metric for this competition is Spearman Rank Correlation Coefficient. The Spearman's rank correlation is computed for each target column, and the mean of these values is calculated for the submission score. The Predictions are in the range [0, 1]

## Dataset
The Dataset is provided as train and test data. The scores for the model will be evaluated based on the Public and Private test data.
Train Dataset has 6079 data points while Public Test Dataset has 476 data points. The Private Test Data is not disclosed.
The dataset contains three text based columns namely question_title, question_body and answer.


The training data has 30 target variables. The values of these variables are to be predicted for a given question-answer pair.
