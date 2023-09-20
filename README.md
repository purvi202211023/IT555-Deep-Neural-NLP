# IT555-Deep-Neural-NLP
## Word2Vec based Model for peS2o Dataset
This repository contains a Jupyter notebook that demonstrates the training of a Word2Vec based model on the peS2o dataset. The dataset consists of research papers from the Computer Science domain.
### Key Features:
**Dataset Selection**: Only research papers from the Computer Science domain are considered.\n2. **Data Split**: A random training dataset of 3000 documents and a test dataset of 1000 documents are used.\n3. 
**Linguistic Unit**: Sentences are used as the linguistic unit for embedding, meaning we embed entire sentences rather than individual words.\n4. 
**Pre-processing**: The input context matrix undergoes a thorough cleanup which includes the removal of:   
- Stopwords
- URLs
- Bullets
- Apostrophes
- Hyphens
- Enumerations
- Numerical-to-text conversion (using `num2words`)
- Punctuations\n5.
- **Initialization of Context Matrix**:
- The context matrix is initialized using tf-idf based vector modeling.
### Libraries and Dependencies:
`num2words`: Used for converting numbers to words. 
`nltk`: For natural language processing tasks such as tokenization and stopword removal.
`sklearn`: Specifically, the `TfidfVectorizer` is used for tf-idf based vector modeling.
`pandas`: For data manipulation.
`numpy`: For numerical operations.
### Getting Started:
1. Install the required libraries:```bash\npip install num2words nltk sklearn pandas numpy```
2. Download necessary `nltk` data:```python\nimport nltk\nnltk.download('punkt')\nnltk.download('stopwords')```
3. If you are using Google Colab, you can mount your Google Drive to access the dataset:```python\nfrom google.colab import drive\ndrive.mount('/content/drive')```
4. Load the dataset and follow the instructions in the notebook to train the model.
### Acknowledgements:
The project is based on the peS2o dataset which consists of research papers from the Computer Science domain.
