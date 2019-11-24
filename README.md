# SemanticProcessing
NLP Topics


##### Concepts and Terms

--Terms act as handles to concepts and the notion of ‘concepts’ gives us a way to represent the ‘meaning’ of a given text.

##### Predicate

--predicate gives us a simple model to process the meaning of complex statements,processing meaning involves understanding the associations between entities.  For e.g. "A football team is comprised of 11 players" is an example of relation type =1 (since there is only one entity type - football players), though the relationship instance is 11 (since there are 11 instances of the entity).

--A predicate is a function which takes in some parameters and returns True or False depending on the relationship between the parameters. For example, a predicate teacher_teaches_course(P = professor Mohan, C = Semantic analysis) returns True.

##### Reification
-- reification refers to combining multiple entity types to convert them into lower order predicates. 

##### Schema
--Schema.org is a joint effort by Google, Yahoo, Bing and Yandex (Russian search engine) to create a large schema relating the most commonly occurring entities on web pages. The main purpose of the schema is to ease search engine querying and improve search performance.

##### Semantic Associations
--**isa**
"a Rose is a flower" 

--**has a **
"a hotel has a rating"

##### Aboutness
--When machines are analysing text, we not only want to know the type of semantic associations ‘is-a’ and ‘is-in’ but also want to know what is the word or sentence about

Croatia fought hard before succumbing to France's deadly attack; lost the finals 2 goals to 4.’

for example, detect that the game is football by defining semantic associations such as “Croatia” is-a “country”, “France” is-a “country”, “finals” is-a “tournament stage”, “goals” is-a “scoring parameter” and so on.


####  five kinds of relationship between different words can be grouped as follows:

##### Hypernyms and hyponyms: 
--This shows the relationship between a generic term (hypernym) and a specific instance of it (hyponym). For example, the term ‘Punjab National Bank’ is a hyponym of the generic term ‘bank’

##### Antonyms: 
--Words that are opposite in meanings are said to be antonyms of each other. Example hot and cold, black and white etc.

###### Meronyms and Holonyms: 
--A term ‘A’ is said to be a holonym of term ‘B’ if ‘B is part of ‘A’ (while the term ‘B’ is said to be a meronym of the term ‘A’). For example, an operating system is part of a computer. Here, ‘computer’ is the holonym of ‘operating system’ whereas ‘operating system’ is the meronym of ‘computer.

###### Synonyms: 
--Terms that have a similar meaning are synonyms to each other. For example, ‘glad’ and ‘happy’.

##### Homonymy and polysemy: 
--Words having different meanings but the same spelling and pronunciations are called homonyms. For example, the word ‘bark’ in ‘dog’s bark’ is a homonym to the word ‘bark’ in ‘bark of a tree’. Polysemy is when a word has multiple (entirely different) meanings. For example, consider the word 'pupil'. It can either refer to students or eye pupil, depending upon the context in which it is used.

##### Principle of Compositionality
--consider how two words are often put together to form a phrase. The semantics of the combination of these words could be very different than the individual words. For example, consider the phrase - ‘cake walk’. The meanings of the terms 'cake' and 'walk' are very different from the meaning of their combination.

##### WordNet 
--is a part of NLTK ,it is used to identify the 'correct' sense of a word.
-- WordNet has a network of synonyms called synset for individual words.

##### ConceptNet 
--is a representation that provides commonsense linkages between words. For example, it states that bread is commonly found near toasters. These everyday facts could be useful if, for e.g., you wanted to make a smart chatbot which says - “Since you like toasters, do also like bread? I can order some for you.”

##### Word Sense Disambiguation - Naive Bayes
-- Word sense disambiguation (WSD) is the task of identifying the correct sense of an ambiguous word such as 'bank', 'bark', 'pitch' etc.and Naive Bayes classifier is Supervised techniques

 #### Word Sense Disambiguation - Lesk Algorithm
--As with most machine learning problems, lack of labelled data is a common problem in building disambiguation models. Thus, we need unsupervised techniques to solve the same problem.  

 A popular unsupervised algorithm used for word sense disambiguation is the Lesk algorithm.
 
 
 ##### Distributional Semantics
 --‘You shall know a word by the company it keeps’.
 
 ##### The most commonly used representation of words is using 'word vectors'. There are two broad techniques to represent words as vectors:

--The term-document occurrence matrix, where each row is a term in the vocabulary and each column is a document (such as a webpage, tweet, book etc.)  

--The term-term co-occurrence matrix, where the ith row and jth column represents the occurrence of the ith word in the context of the jth word.


##### There are two ways of creating a co-occurrence matrix:

##### Using the occurrence context (e.g. a sentence):
Each sentence is represented as a context (there can be other definitions as well). If two terms occur in the same context, they are said to have occurred in the same occurrence context.

###### Skip-grams (x-skip-n-grams):
A sliding window will include the (x+n) words. This window will serve as the context now. Terms that co-occur within this context are said to have co-occurred.
 


