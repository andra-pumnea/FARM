In order to fine-tune a language model or train it from scratch on a custom dataset, the following format is required: 
- one sentence per line (sentence segmentation). Example tools for this are: Spacy and NLTK. 
- one newline between documents
- optionally: shuffle the sentences within the documents (not within the dataset!)
- make sure that each dataset has at least 500MB, otherwise the resulting model might not be meaningful

Here is an overview of the required format:

[Doc2]
Sentence 1
Sentence 2
…
[Doc3]
Sentence 1
Sentence 2
…
[Doc1]
Sentence 1
Sentence 2


Here is an example: