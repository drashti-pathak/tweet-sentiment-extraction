

# ROBERTA
## Summarising BERT
BERT takes as input a concatenation of two segments (sequences of tokens), x1, . . . , xN and y1, . . . , yM. 
Segments usually consist of more than one natural sentence. 
The two segments are presented as a single input sequence to BERT with special tokens delimiting them: [CLS], x1, . . . , xN , [SEP], y1, . . . , yM, [EOS]. 
M and N are constrained such that M + N < T, where T is a parameter that controls the maximum sequence length during training. 

The model is first pretrained on a large unlabeled text corpus and subsequently finetuned using end-task labeled data. 

### Training Objectives
```
During pretraining, BERT uses two objectives: 
    • masked language modeling and 
    • next sentence prediction.
```
### Masked Language Model (MLM) 
    • A random sample of the tokens in the input sequence is selected and replaced with the special token [MASK]. 
    • The MLM objective is a cross-entropy loss on predicting the masked tokens. 
    • BERT uniformly selects 15% of the input tokens for possible replacement. Of the selected tokens, 80% are replaced with [MASK], 10% are left unchanged, and 10% are replaced by a randomly selected vocabulary token.
    • In the original implementation, random masking and replacement is performed once in the beginning and saved for the duration of training, although in practice, data is duplicated so the mask is not always the same for every training sentence (see Section 4.1). 
### Next Sentence Prediction (NSP) 
    • NSP is a binary classification loss for predicting whether two segments follow each other in the original text. 
    • Positive examples are created by taking consecutive sentences from the text corpus. Negative examples are created by pairing segments from different documents.
    • Positive and negative examples are sampled with equal probability. 
    • The NSP objective was designed to improve performance on downstream tasks, such as Natural Language Inference (Bowman et al., 2015), which require reasoning about the relationships between pairs of sentences. 



## Changes made in Roberta
