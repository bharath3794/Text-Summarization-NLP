# Text-Summarization-NLP
Summarized customer reviews from Amazon Fine Food Reviews Dataset using Encoder-Decoder Architecture

## Dataset
https://snap.stanford.edu/data/web-FineFoods.html

#### Sample Data
<img src="https://github.com/bharath3794/Text-Summarization-NLP/blob/main/images/dataset.PNG">


## Model Architecture
Encoder-Decoder Architecture with RNN Units (GRU's) used in both Training and Testing phases
#### Training
<img src="https://github.com/bharath3794/Text-Summarization-NLP/blob/main/images/NLP_Training.jpg" width=70% height=70%>

#### Testing
<img src="https://github.com/bharath3794/Text-Summarization-NLP/blob/main/images/NLP_Testing.jpg" width=70% height=70%>


## Model Summary
<img src="https://github.com/bharath3794/Text-Summarization-NLP/blob/main/images/model_summary.PNG" width=70% height=70%>

## Evaluation
#### Metrics Used
Precision, Recall, F-1 Measure with ROUGE-1, ROUGE-2 and ROUGE-L.
ROUGE (Recall-Oriented Understudy for Gisting Evaluation)
ROUGE-1: This checks for the unigram overlap of words between machine generated summary and reference summary.
ROUGE-2: This checks for the bigram overlap of words between machine generated summary and reference summary.
ROUGE-L: This measures the longest matching sequence of words between machine generated summary and reference summary.

#### Results
Trained on 548,000 samples
Tested on 2500 samples using ROUGE Implementation
##### Tested Example:-
###### Part of the original text: 
``this is a tasty drink, a small 8 ounce can contain relatively high 140 calories. the price isn’t a bargain.At nearly $1 per can, it wouldn't seem to be a compelling value.``
###### Reference Summary: 
``tasty but relatively high in calories``
###### Machine Generated Summary: 
``tasty but not a great value``
#### Precision, Recall, F-1 Measure with ROUGE-1, ROUGE-2 and ROUGE-L
<img src="https://github.com/bharath3794/Text-Summarization-NLP/blob/main/images/results.PNG" width=40% height=40%>
