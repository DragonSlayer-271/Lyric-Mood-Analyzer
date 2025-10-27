# Lyric-Mood-Analyzer

### Team Members
* Stella Asanova 
* Jillienne Lapid `@jilliennelapid`
* Rose Montgomery
* Brian Tran
___

## Project Description
Lyrics mood analyzers usually analyze the entire song and give it a single emotional label, and the ones that go line by line often ignore musical structure. There isn’t anything that shows how artists shift moods across different sections of the song. Our objective is to have the model analyze emotions and how they change/develop throughout the song, based on musical structure. 

Since we are analyzing based on the lyrics (which is textual data), NLP will be very important. We plan on using it for the emotional classification of each musical section. As well as contextual understanding of the lyrics to understand what contributes to the emotional meaning of the lyrics. Additionally, we will use it for Temporal/Sequential Analysis, so we can model emotion transitions across sections. As well as Text Summarization and Feature Extraction, we can identify what features influence the emotions. 

### Model Architecture
We chose a combination of classical NLP methods and deep NLP models. The classical is easy to implement and fast to train. Using TF-IDF and SVM for baseline classifiers to establish emotion classification. Additionally, we will use TF-IDF features to vectorize section text and use SVM to classify section emotion. However, the classical NLP methods have limitations and cannot get context and sequential meaning. This is where deep NLP models will be important to use. Although it requires more resources, it is context-aware. We will be using pretrained BERT-based models to contextualize vector representation and extract tokens, and feed these embeddings into a classifier. And we will be using BiLSTM or Transformer Encoder over Sections to model emotion transitions over sections. Using embeddings from BERT to learn temporal patterns and extract emotional labels for each section. This will be important for understanding how emotions evolve across sections. 

### Data Used
We are using textual data, which is the lyrics of songs. Each song's lyrics have a musical structure of chorus, verse, and bridge. This is why the main importance will be with the deep NLP models. We can model section-to-section emotional flow with encoders such as BiLSTM or Transformer. We can use contextual embeddings like BERT. Since our data set is structured and we want to see what happens throughout the lyrics, simply using classical NLP methods would not be enough. Though we plan to utilize some classical NLP methods, the main goal is to understand emotional dynamics, which deep NLP models align more with. 

### How to run
How to run will go here
