# hate-speech-detection-nlp
Developed a Hate Speech Detection model that can accurately classify tweets as Hate Speech, Offensive, or Neither.

Hate speech detection is a crucial task in Natural Language Processing (NLP), aimed at identifying harmful and offensive content in textual data. My study explores various techniques for text preprocessing, feature extraction, and classification to build an effective hate speech detection model. The dataset used consists of labeled tweets categorized as Hate Speech, Offensive Language, or Neither. The preprocessing phase involves text normalization, stopword removal, POS tagging, and dependency parsing to enhance the quality of input data.
For feature extraction, TF-IDF and FastText embeddings were utilized, where TF-IDF captures statistical word importance, and FastText embeddings retain contextual meaning using subword information.

Dataset:

There are numerous dataset available online for hate speech detection. I have chosen a multiclass dataset from the Kaggle website.
Dataset link: Hate Speech and Offensive Language Detection
Credits: tdavidson/hate_speech_offensive · Datasets at Hugging Face
This dataset is a csv file that has 24784 entries which are collected from Twitter(X) users tweets. It has a tweet column that has the data.  
The Class column in this dataset classifies tweets into
0 - hate speech
1- offensive language 
2- neither 

The dataset also contains columns for annotations given by other people for each tweet as count(total annotations), hate_speech_count, offensive_language_count and neither_count.
I have used Google Collab to load the dataset and preprocess it. Initially, I downloaded necessary modules and imported them beforehand. It includes sentence-transformers, CountVectorizer, TfidfVectorizer, Stopwords, etc.
I have done preprocessing and EDA.
The preprocessing steps transformed raw text into structured data by lowercasing, removing retweets, usernames, punctuation, and stopwords. POS tagging and dependency parsing were applied to extract linguistic features, which were vectorized using TF-IDF.
For semantic understanding, FastText embeddings were used to create a word representation by averaging word vectors in each tweet. This approach captures contextual meaning and handles out-of-vocabulary words effectively.

Also built a traditional classifier using Logistic Regression and built a simple Multi Layer Perceptron model and evaluated and compared the results.
