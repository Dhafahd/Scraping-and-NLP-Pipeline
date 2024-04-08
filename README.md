### MST AIDS 2023-2024 (Département Génie Informatique)
### Subject : The main purpose behind this lab is to get familiar with Scraping and NLP Pipeline.
### Realize by : Chibani Fahd
### web source : Aljarida24r
### Model : NLP
#
#
#### There are two parts to this work, and each part is contained in a notebook.
#
## PART I :  Scraping and storing data 
#
#### In this project segment, we harnessed the power of BeautifulSoup, a Python library renowned for web scraping, to extract a multitude of articles—comprising links, titles, and content—from the Aljarida24 website. Subsequently, we orchestrated the seamless integration of MongoDB, a versatile NoSQL database, to meticulously store this extracted information. MongoDB's flexible document-oriented architecture facilitated the storage of varied article attributes in a structured format, ensuring scalability and ease of access. By employing a combination of BeautifulSoup and MongoDB, we engineered a proficient solution for aggregating and persisting article data from Aljarida24, empowering future analyses and applications with a rich repository of pertinent information.
#
![image](https://github.com/Dhafahd/Scraping-and-NLP-Pipeline./assets/114614233/c9a06cd3-03b1-4387-bdf7-a663d36219af)
#
## PART II :  NLP Pipeline
#
#### In this section, we'll explore the intricate stages of the Natural Language Processing (NLP) pipeline, encompassing tasks such as tokenization, part-of-speech tagging, Stop words, Discretization,
Normalization, Stemming, Lemmatization and more,elucidating the sequential flow of text processing from raw input to insightful analysis.
To test this different technique we chose to work on one article
#
### 1) Establishment of NLP Pipeline 
#
#### Text Cleaning: This involves preprocessing the text to remove any irrelevant or noisy elements, such as special characters, punctuation, HTML tags, or non-Arabic characters, ensuring that the text is in a clean and readable format for further analysis.
#### Tokenization: Tokenization is the process of breaking down the text into smaller units called tokens, which can be words, phrases, or symbols. In Arabic text, tokenization involves splitting the text into individual words or morphemes, considering the unique properties of Arabic script, such as the presence of diacritics and the non-separation of words by spaces.
#### Stop Words: Stop words are common words that are often filtered out during text processing because they typically do not carry significant semantic meaning. In Arabic NLP, stop words may include common functional words like prepositions, conjunctions, and pronouns, which can be excluded from analysis to focus on more meaningful content.
#### Discretization: Discretization involves converting continuous or numerical data into discrete categories or bins. In the context of Arabic text analysis, discretization might be applied to features such as word frequencies or sentiment scores to categorize them into specific ranges or levels, facilitating further analysis or interpretation.
#### Normalization: Normalization refers to the process of standardizing text data to a common form or representation, which helps reduce variations and ensure consistency across different documents or sources. In Arabic NLP, normalization may involve tasks such as removing diacritics, normalizing letter forms, handling different dialects or spellings, and converting text to a standardized encoding format like UTF-8.
#
### 2) Stemming and Lemmatization
#
#### Stemming: Stemming is a text normalization technique that aims to reduce words to their root or stem form by removing affixes. In Arabic, stemming algorithms typically truncate word endings to obtain the stem, but they may not always produce linguistically valid roots due to the complex morphology of Arabic words. Stemming algorithms in Arabic NLP often use rules-based approaches or dictionary lookups to perform stemming.
#### Lemmatization: Lemmatization, on the other hand, involves reducing words to their canonical or dictionary form, known as the lemma. Unlike stemming, lemmatization considers the morphological and syntactic context of words, ensuring that the resulting lemma is a valid word form. In Arabic NLP, lemmatization algorithms leverage linguistic resources such as dictionaries, morphological analyzers, and part-of-speech tagging to accurately derive lemmas.
#
### 3) Parts of Speech technics based on both Rule based and Machine learning approaches.
#
### Rule-Based Approaches:
Rule-based POS tagging relies on predefined linguistic rules and patterns to assign parts of speech to words in a sentence. These rules are often crafted by linguists or domain experts based on language-specific grammatical structures. Some common techniques in rule-based POS tagging include:
Lexical Lookup: Assigning parts of speech based on the word itself and its context. This may involve using dictionaries or lexicons that list words along with their likely POS tags.
Morphological Analysis: Analyzing the morphology of words, such as suffixes, prefixes, and word endings, to infer their grammatical categories. Rules are formulated to identify patterns indicative of certain parts of speech.
Contextual Rules: Applying rules based on syntactic and semantic context to disambiguate POS tags. For example, determining the POS tag of a word based on its neighboring words or its role in the sentence structure.
Rule-based approaches are often transparent and interpretable, as the tagging decisions are based on explicit rules. However, they may struggle with handling ambiguity and capturing complex linguistic phenomena.
#
### Machine Learning Approaches:
Machine learning-based POS tagging involves training statistical models on annotated corpora, where each word in the training data is labeled with its correct POS tag. These models then learn patterns and associations between words and their POS tags, which are used to predict tags for unseen text. Common machine learning techniques for POS tagging include:
Hidden Markov Models (HMMs): Modeling the sequence of POS tags in a sentence and the emission probabilities of words given their POS tags. HMMs estimate the most likely sequence of POS tags for a given sentence.
Conditional Random Fields (CRFs): Discriminative models that capture dependencies between input features (e.g., words, context) and output labels (POS tags). CRFs consider the entire input sequence when making tagging decisions.
Neural Network Architectures: Deep learning approaches, such as recurrent neural networks (RNNs), long short-term memory networks (LSTMs), and transformer-based models, have shown promise in POS tagging by capturing long-range dependencies and contextual information.
Machine learning approaches often excel in capturing complex patterns and generalizing to diverse linguistic contexts. They can handle ambiguity more effectively than rule-based systems but may lack transparency in their decision-making process.
#
### 4) NER Methods.
#
#### Named Entity Recognition (NER) is a crucial task in natural language processing that involves identifying and categorizing named entities (e.g., person names, organization names, locations, dates) within text. Various methods and techniques are employed for NER, including:
Rule-Based Approaches:
Rule-based NER systems rely on handcrafted rules and patterns to identify named entities in text. These rules may involve regular expressions, lexical lookup, syntactic patterns, and contextual cues. For example, a rule-based system might identify organization names by looking for capitalized words followed by certain keywords like "Inc." or "Corp." Rule-based approaches offer transparency and interpretability but may be limited in handling complex linguistic variations and new entity types.
Dictionary-Based Methods:
Dictionary-based NER systems utilize curated dictionaries or lexicons containing lists of known named entities along with their categories (e.g., person, organization, location). These dictionaries are often augmented with additional information such as aliases, variations, and context-specific cues. During NER, text is scanned for matches against entries in the dictionary, and identified entities are tagged accordingly. While effective for recognizing known entities, dictionary-based methods may struggle with identifying novel or rare entities absent from the lexicon.
Statistical and Machine Learning Approaches:
Statistical and machine learning methods for NER involve training models on annotated corpora, where each word is labeled with its corresponding named entity category. 
Common machine learning algorithms used for NER
#
### 5) Synthesis
#
####  This first lab was a great opportunity to get familiar with the difference libraries of Scraping and  techniques of storing data in the database in addition of NLP Pipeline that we have seen in during class from Text Cleaning and Tokenization to Parts of Speech and NER Methods by using them in Arabic paragraph which was a bit difficult but we get to know this technologies more


