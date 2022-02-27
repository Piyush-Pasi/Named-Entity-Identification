# Implementing Named Entity Identification using SVM
To identity if a word is a named entity (NE) or not using Support Vector Machine Classifier. Code & data files can also be downloaded at [link](https://drive.google.com/file/d/1KvPj-QWDxBco0Dil4bPH2JUnXtchlHr6/view?usp=sharing)


*Platform* : Python Jupyter, Google Colab or VS Code.  
VS Code (version 1.59.0) was used to run the code. 

## Common libraries used in HMM based implementation of WSD
numpy (version 1.19.5)  
pickle (version 4.0)  
regex (version 2019.12.20)  
sklearn (version 0.24.2)  
datasets library is used

## Running NEI_SVM.ipynb

*Run all the cells* for training and testing of SVM model.

## Features added
- More features added: binary features like is next word NE, is previous word NE, does previous word starts with Capital letter, and so on... (see comments in code)
- Two pass SVM added: In 1st pass predict NE or not. Use these for 2nd pass in test time to check if next word is NE or not (as next word output not available during test time)
- Feature normalization  
- Top 20 feature analysis  
- SVM with word embeddings added

###### Caution:
Run all cells for functions to be defined, Note and Cautions are mentioned in the Notebook as well

##### References
https://paperswithcode.com/dataset/conll-2003

https://huggingface.co/datasets/viewer/?dataset=conll2003

https://medium.com/@bedigunjit/simple-guide-to-text-classification-nlp-using-svm-and-naive-bayes-with-python-421db3a72d34

http://www.scielo.org.mx/scielo.php?script=sci_arttext&pid=S1405-55462016000300495#t1

https://towardsdatascience.com/named-entity-recognition-and-classification-with-scikit-learn-f05372f07ba2

http://citeseerx.ist.psu.edu/viewdoc/download;jsessionid=7825E40C84F50518A02A5AF09A53DEE1?doi=10.1.1.309.6052&rep=rep1&type=pdf
