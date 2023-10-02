# IT555-Deep-Neural-NLP
## Word2Vec based Model for peS2o Dataset
This repository contains a Jupyter notebook that demonstrates the training of a Word2Vec based model on the peS2o dataset. The dataset consists of research papers from the Computer Science domain.
### Key Features:

**Dataset Selection**: Only research papers from the Computer Science domain are considered. 

**Data Split**
- A random training dataset of 3000 documents and a test dataset of 1000 documents are used.

**Linguistic Unit**
- Sentences are used as the linguistic unit for embedding, meaning we embed entire sentences rather than individual words.

**Pre-processing**: The input context matrix undergoes a thorough cleanup which includes the removal of  
- Stopwords
- URLs
- Bullets
- Apostrophes
- Hyphens
- Enumerations
- Numerical-to-text conversion (using `num2words`)
- Punctuations
  
**Initialization of Context Matrix**
- The context matrix is initialized using tf-idf based vector modeling.
### Libraries and Dependencies:
`num2words`: Used for converting numbers to words. 
`nltk`: For natural language processing tasks such as tokenization and stopword removal.
`sklearn`: Specifically, the `TfidfVectorizer` is used for tf-idf based vector modeling.
`pandas`: For data manipulation.
`numpy`: For numerical operations.

- Perform testing on multiple similar words.

### Acknowledgements:
The project is based on the peS2o dataset. From this dataset we took only those research papers that are from the Computer Science domain.
