In order to fine-tune a FARM model on a NER task, your dataset will need to be in one of the following formats: 
- IOB1 (conll03), germEval2014, IOB2.
- if the dataset is neither IOB1 or germEval2014, it is automatically assumed to be in IOB2 format. 
- IOB1, IOB2:
    - first column is the word, last column is the label (entity)
    - columns are space separated
- germEval2014:
    - second column is the word, second to last column is the label (entity). This is because FARM takes only the first level of labels for this format and 
    ignores the second level
    - columns are tab separated
- all formats assume one word per line 
- sentences are separated through a newline
- in general, you should be able to define your own delimiter in the  NERProcessor block

Here is an example: