# Data Mining: Assignment 2
### Maria Fritzela
***
Classifying text data from articles of 5 different categories: <br>
(business, entertainment, politics, sport, tech)

### About the data given

Dataset consists of 2225 documents from a news website 
corresponding to stories in five topical areas from 2004-2005.<br>
First line of each txt file is the title of the article.<br>
Dataset file tree: 

````
data-mining-assignment-2
├── ergasia2.ipynb
├── fulltext
│   └── data
│       ├── business
│               ├── 001.txt
│               ├── ...
│               └── 510.txt
│       ├── entertainment
│               ├── 001.txt
│               ├── ...
│               └── 386.txt
│       ├── politics
│               ├── 001.txt
│               ├── ...
│               └── 417.txt
│       ├── sport
│               ├── 001.txt
│               ├── ...
│               └── 511.txt
│       ├── tech
│               ├── 001.txt
│               ├── ...
│               └── 401.txt
│       └── README.TXT
````

### Task 0: Creation of TSV files

- Create file **train_set.tsv** (80%)<br>
  Columns: id, title, content, category 
- Create file **test_set.tsv** (20%)<br>
  Columns: id, title, content
- Create file **dataset.tsv**<br>
  Columns: id, title, content, category 

### Task 1: Wordcloud creation

Creation of one wordcloud for each category of articles, using the text from all articles of that category found in the dataset

### Task 2: Data Classification

#### A) Text pre-processing
Using tokenization and stop-word filtering, then creating the bag-of-words and TF/IDF vector for our data

#### B) Classification
Trying the following classification methods:
- Support Vector Machines
- Random Forest
- Naive Bayes
- Self-made K-Nearest Neighbor estimator (scikit-learn-compatible)

#### C) Scores
Using the following methods
- Precision
- Recall
- F-Measure
- Accuracy
- ROC plot

### Task 3: Beat the Benchmark

Using lemmatization of words to improve the scores from the previous question.

### Task 4: Clustering

Creation of clustering of BoW, TFIDF, and Document-Embeddings arrays of dataset using K-means clustering with Cosine Similarity.
- Create vectors
- Reduce the dimensionality of the vectors using PCA, SVD and ICA, to make 2-d plotting possible
- Clustering

