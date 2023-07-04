# Topic Modeling Methods LDA and BTM for Uncovering Topics in Open-Ended Employee Engagement Survey Responses 

## Description

This Github is created to support a thesis project of Applied Data Science. A description is given of the research question, the steps undertaken and the result: 

The research focused on exploring the effectiveness of topic modeling methods, specifically LDA and BTM. The research aim was to answer the following question: “Are the topic modeling methods LDA and BTM effective to use to gain insight in the topics present in unstructured  answers to open ended questions in employee engagement surveys?” Firstly, the data is preprocessed to create a clean and tidy dataset that served as an input for the topic modeling methods. Then, the parameters are optimized. The optimization of parameters played a crucial role in achieving meaningful results. Theoretically grounded methods helped in making a choice in the best number of topics fitting the data. The parameters that put weights on how the documents are composed and how the topics are composed, were tuned through a grid search by comparing the coherence scores. The two models with optimized parameters are performed by using developed packages in Python and R. The models are evaluated on their coherence scores, on the possibility of human interpretation of the topics and on eyeballing to assess the distinctiveness and specificity of the topics. The overall performance of the BTM model was way better than the LDA model.  

## Programming language

The code were performed using R Statistical Software (v4.2.1; R Core Team 2023). The analysis of the BTM model was performed with Python (v3.10.12; Python Software Foundation 2023). 

## The files

All files are self-explaining and the required packages are ready to download and to open in each file. 

It is important to run the preprocessing file first (Preprocessing.Rmd), this prepared the data for usage in all the other files. 

All the other RMD and ipynb files can be run independently after the preprocessing. 

Tuning parameters BTM.ipynb --> This ipynb file can be used to determine the optimal topics k and the parameters alpha and beta of the LDA model. 
BTM model.ipynb --> With this ipynb file the BTM model can be run. 
Tuning parameters LDA.Rmd --> This rmd file can be used to determine the optimal topics k and the parameters alpha and beta of the LDA model. 
LDA model.Rmd --> With this ipynb file the LDA model can be run. 

## Usage

These files can be used to analyze unlabeled text data. This research was focused on identifying topics of unstructured answers on various open questions. The dataset used has two columns "question_text" and "answer". 

Example:
question_text: Wat kan *Bedrijf* doen om jouw betrokkenheid te vergroten?
answer: Improve on local presence Equality for women

## Topiclist

The aim of this research was to create a topiclist that could be used for analyzing open answers of an engagement monitor. The BTM model served as base for creating a topic list. 16 topics are included in the list with some manual adjustments in adding and deleting topics and words. This topiclist can be found in this Github as the "Topiclijst.csv" file. The rmd file "Example of answer analyzing.Rmd" gives examples on how to use the topic list in analyzing open-ended answers. It is important to note that these are just ideas and are not theoretically grounded. 



