# NLP-Authorship-Latin-Eng
Automating Latin-English Authorship Attribution. 

Acess the tentative report here: LINK

## Dataset

* The dataset includes 101,000 Latin-English text pairs from 57 classical books, with a 99%/1%/1% train/validation/test split.
* Text distribution across books is heavily skewed; top 5 most common books were selected and equalized to reduce the dataset to approximately 4,400 entries for fair model training.
* Implemented back-translation to augment the dataset, increasing its size to approximately 17,000 entries by translating texts to Italian and back to English, then to French and back, resulting in 17,352 texts.

* Used the Lingua Language Detector to filter out texts not in the correct language, removing erroneous entries across all data instances.

* Expanded all contractions in the dataset using word’s movers distance for English and specific rules for Latin to handle multi-semantic contractions.

* Employed NLTK libraries for English data pre-processing (lemmatization and stop word removal) and CLTK libraries for Latin text, summarizing pre-processing steps for each data version.


## Exploration
Folder containing Python notebooks of the data exploration of the models examined and figures outputted by those models. 
*  [CNN](https://github.com/sghassemlou/NLP-Authorship-Latin-Eng/blob/main/Exploration/Models/CNN_550.ipynb)
*  [RNN](https://github.com/sghassemlou/NLP-Authorship-Latin-Eng/blob/main/Exploration/Models/RNN.ipynb)
*  [SVM](https://github.com/sghassemlou/NLP-Authorship-Latin-Eng/blob/main/Exploration/Models/SVMipynb)
*  [mBERT](https://github.com/sghassemlou/NLP-Authorship-Latin-Eng/blob/main/Exploration/Models/mBERT.ipynb)

### Sample Figures
#### CNN Accuracies
![alt text](https://github.com/sghassemlou/NLP-Authorship-Latin-Eng/blob/main/Exploration/CNNAcc.png?raw=true "CNN Accuracies")
#### RNN Accuracies
![alt text](https://github.com/sghassemlou/NLP-Authorship-Latin-Eng/blob/main/Exploration/RNNacc.png?raw=true "RNN Accuracies")
