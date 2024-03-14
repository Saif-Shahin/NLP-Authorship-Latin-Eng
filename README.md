# NLP-Authorship-Latin-Eng
Automating Latin-English Authorship Attribution. 

Acess the tentative report here: LINK

## Dataset Summary and Preprocessing

- **Dataset Composition**: Includes 101,000 Latin-English text pairs from 57 classical books.
- **Data Split**: Utilizes a 99%/1%/1% train/validation/test split.
- **Text Distribution**: Initially heavily skewed across books; adjusted by selecting and equalizing entries from the top 5 most common books, reducing the dataset to approximately 4,400 entries.
- **Back-Translation Augmentation**:
  - Increased dataset size to approximately 17,000 entries through back-translation.
  - Process involved translating texts to Italian and then back to English, followed by further translation to French and back, totaling 17,352 texts.
- **Language Accuracy**:
  - Employed the Lingua Language Detector to identify and filter out incorrect language texts, enhancing dataset quality.
- **Contraction Expansion**:
  - Expanded all contractions in the dataset using word’s movers distance for English and specific rules for Latin, addressing multi-semantic contractions.
- **Preprocessing Steps**:
  - Used NLTK libraries for lemmatizing and removing stop words from the English data.
  - Applied CLTK libraries for similar preprocessing on the Latin text.


## Exploration
Folder containing Python notebooks of the data exploration of the models examined and figures outputted by those models. 
*  [CNN](https://github.com/sghassemlou/NLP-Authorship-Latin-Eng/blob/main/Exploration/Models/CNN_550.ipynb)
*  [RNN](https://github.com/sghassemlou/NLP-Authorship-Latin-Eng/blob/main/Exploration/Models/RNN.ipynb)
*  [SVM](https://github.com/sghassemlou/NLP-Authorship-Latin-Eng/blob/main/Exploration/Models/SVMipynb)
*  [mBERT](https://github.com/sghassemlou/NLP-Authorship-Latin-Eng/blob/main/Exploration/Models/mBERT.ipynb)

## Results

<img width="800" alt="Screen Shot 2024-03-14 at 4 14 43 PM" src="https://github.com/Saif-Shahin/NLP-Authorship-Latin-Eng/assets/90293080/df3c545c-a705-4a93-8786-95fb1a82bd96">

