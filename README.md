# 100_NLP_challenge
My solutions for the 100 NLP drill exercises from Tohoku University in Japan

Chapter 1: Preparation Movement
00. Reverse order of character strings
Obtain the character string of the character string "stressed" arranged in reverse (from the end to the beginning).

01. "Patatokukashie" (「パタトクカシーー」)
Retrieve the 1st, 3rd, 5th and 7th characters of the character string "Patatokukashie" (「パタトクカシーー」) and obtain a concatenated character string.

02. "Police Car" + "Taxi" = "Patatokukasy" (「パトカー」＋「タクシー」＝「パタトクカシーー」)
Connect the characters "patrol car" + "taxi" alternately from the top to obtain the character string "Patatokukassei" (「パトカー」＋「タクシー」＝「パタトクカシーー」).

03. Pi
Please break down the sentence "Now I need a drink, alcoholic of course, after the heavy lectures involving quantum mechanics." Into words and create a list in which the (alphabetical) number of characters of each word is arranged in order of appearance.

04. Element symbol
"Hi He Lied Because Boron Could Not Oxidize Fluorine. New Nations Might Also decompose the sentence" Sign Peace Security Clause. Arthur King Can. "Into words, 1, 5, 6, 7, 8, 9, 15, 16, 19 The first word of the first word is extracted, the other word is taken at the beginning, and an associative array (dictionary type or map type) from the extracted character string to the position of the word (what number from the beginning) Make it.

05. n-gram
Create a function that creates an n-gram from a given sequence (string, list, etc.). Using this function, obtain the word bi-gram and the character bi-gram from the sentence "I am an NLPer".

06. Set
Find the set of character bi-grams contained in "paraparaparadise" and "paragraph" as X and Y respectively and find the union, intersection, and difference set of X and Y. Also check if the bi-gram 'se' is included in X and Y.

07. Sentence generation by template
Implement a function that takes the arguments x, y, z and returns the string "y at times x". Furthermore, let x = 12, y = "air temperature", z = 22.4 and confirm the execution result.

08. Cipher text
Implement the function cipher which converts each character of a given character string with the following specifications.

If it is lower case letter (219 - character code) replaced by letter
Other characters are output as they are
Use this function to encrypt and decrypt English messages.

09. Typoglycemia
Create a program that randomly rearranges the order of other characters, leaving the beginning and ending letters of each word for word strings separated by spaces. However, words whose length is 4 or less are not rearranged. Give an appropriate English sentence (eg "I could not believe that I think actually understand what I was reading: the phenomenal power of the human mind.") And confirm the execution result.

Chapter 2: Basics of UNIX Commands
hightemp.txt is a file that stores the record of the highest temperature in Japan in tab-delimited format of "prefecture" "point" "℃" "day". Create a program to perform the following processing and execute hightemp.txt as an input file. Furthermore, execute the same process with the UNIX command and check the execution result of the program.

10. Count the number of rows
Count the number of rows. Use the wc command for confirmation.

11. Replace tabs with spaces
Replace one tab space with one space. To confirm, use sed command, tr command, or expand command.

12. Save column 1 to col1.txt and column 2 to col2.txt
Save only the first column of each row to col1.txt, and extract only the second column as col2.txt in a file. To check, use the cut command.

13. Merge col1.txt and col2.txt
Combine col1.txt and col2.txt created in 12 and create a text file in which the first and second columns of the original file are arranged in tab separator. Use the paste command for confirmation.

14. Output N rows from the beginning
Receive the natural number N by means such as command line argument and display only the first N lines of the input. Use the head command for confirmation.

15. Output the last N rows
Receive the natural number N by means such as command line argument and display only the last N lines of the input. Use the tail command for confirmation.

16. Divide the file into N
Receive the natural number N by means such as command line argument and divide the input file into N by row. Realize the same processing with the split command.

17. Different character strings in the first column
Find the type of string (string of different strings) in the first column. To confirm, use sort, uniq command.

18. Sort each row by descending numerical value of column 3
Arrange each line in the reverse order of the third column number (note: sort the contents of each line without changing it). Use the sort command for confirmation (this problem does not have to match the result when executed with command).

19. Find frequency of occurrence of character strings in the first column of each line and arrange them in descending order of appearance frequency
Find the appearance frequencies of character strings in the first column of each line, and arrange them in descending order of their appearance. To check, use cut, uniq, sort command.

Chapter 3: Regular Expressions
There is a file jawiki-country.json.gz which exported Wikipedia articles in the following format .

One article information is stored in JSON format on one line
In each row, the article name is stored in the dictionary object with the "title" key and the article body in the "text" key, and the object is written out in JSON format
The whole file is compressed with gzip
Create a program to perform the following processing.

20. Reading JSON data
Read the JSON file of the Wikipedia article and display the article body about "UK". In Problem 21 - 29, execute on the article body extracted here.

21. Extract row containing category name
Extract the line declaring the category name in the article.

22. Extract category name
Extract category names of articles (by name, not by line).

23. Section structure
Please display the section name included in the article and its level (eg 1 if == section name ==).

24. Extract file reference
Extract all the media files referenced from the article.

25. Extract template
Extract the field name and value of the "basic information" template included in the article and store it as a dictionary object.

26. Removing emphasis markup
At the time of processing 25, please remove MediaWiki's emphasized markup (all of weak emphasis, emphasis, strong emphasis) from the template value and convert it to text (Reference: Markup Quick Reference Table ).

27. Removing internal links
In addition to the processing of 26, remove MediaWiki's internal link markup from the template value and convert it to text (Reference: Markup Quick Reference Table ).

28. Elimination of MediaWiki markup
In addition to the processing of 27, remove the MediaWiki markup as much as possible from the value of the template and format the basic information of the country.

29. Acquire the URL of the flag image
Use the contents of the template and obtain the URL of the flag image. (Hint: MediaWiki API of imageinfo by calling, it is sufficient to convert the file reference to the URL)

Chapter 4: Morphological Analysis
Morphologically analyze the sentence ( neko.txt ) of Natsume Soseki's novel "I am a cat" with MeCab and save the result in a file named neko.txt.mecab. Using this file, implement the program corresponding to the following questions.

For matters 37, 38 and 39 , use matplotlib or Gnuplot .

30. Read morphological analysis result
Implement a program to read the morphological analysis result (neko.txt.mecab). However, each morpheme is stored in a mapping type whose key is surface type, base type, part of speech (pos), part of speech sub classification 1 (pos 1), and one sentence is expressed as a list of morphemes (mapping type) Do it. In the remaining problems in chapter 4, use the program created here.

31. Verb
Extract all the surface forms of verbs.

32. Original verb form
Extract all original verb forms.

33. Suspicious nouns
Extract all nouns of saga connection.

34. "B of A"
Extract noun phrases in which two nouns are connected with "".

35. Connecting nouns
Extract the concatenation of nouns (nouns that appear consecutively) with the longest match.

36. Frequency of occurrence of words
Find the words appearing in the sentences and their frequency of appearance, and arrange them in descending order of appearance frequency.

37. Top 10 Frequencies
Display 10 words with high frequency of occurrence and its appearance frequency in a graph (eg bar graph).

38. Histogram
Draw a histogram of word appearance frequency (appearance frequency on the horizontal axis, bar graph showing the number of types of words with appearance frequency on the vertical axis).

39. Zipf's law
Plot the log-log graph with the word occurrence frequency ranking on the horizontal axis and its occurrence frequency on the vertical axis.

Chapter 5: Dependency Analysis
Analyze the sentence ( neko.txt ) of Natsume Soseki's novel "I am a cat" with CaboCha and save the result in a file called neko.txt.cabocha. Using this file, implement the program corresponding to the following questions.

40. Reading the dependency analysis result (morpheme)
MorphImplement class representing morpheme . This class has a surface layer shape ( surface), a basic shape ( base), a part of speech ( pos), and a part classification classification 1 ( pos1) in a member variable. In addition, read the analysis result (neko.txt.cabocha) of CaboCha Morph, express each sentence as a list of objects, and display the morpheme string of the third sentence.

41. Reading the result of dependency analysis (clause / dependency)
In addition to 40, Chunkimplement a class representing phrases . This class shall have Morpha list of morphemes ( objects) ( morphs), a clause clause index number ( dst) and a list of source clause index numbers ( srcs) in member variables. Furthermore, read the analysis result of CaboCha of the input text, express one sentence as Chunka list of objects, and display the character string of the clause of the eighth sentence and the partner. In the remaining problems in chapter 5, use the program created here.

42. Display of the source and destination clause
Extract all texts of the source clause and the clause of the partner in the tab delimited format. However, please do not output symbols such as punctuation marks.

43. Extraction of clauses including nouns pertaining to phrases containing verbs
If a phrase containing a noun relates to a phrase containing a verb, extract them in a tab-delimited format. However, please do not output symbols such as punctuation marks.

44. Visualization of dependency trees
Visualize the dependency tree of a given sentence as a directed graph. The visualization, the dependency tree DOT language converted into, Graphviz preferably used. You can also use pydot to directly visualize a directed graph from Python .

Extraction of case pattern of verb
I would like to investigate the cases that Japanese predicates can take, considering the sentence being used this time as a corpus. Predicate a verb, think the sentence of a phrase related to a verb as a case, and output the predicate and case in a tab delimited format. However, the output should satisfy the following specifications.

In a phrase including a verb, the basic form of the leftmost verb is used as a predicate
Position the particle of the predicate
When there are two or more particles (phrases) related to a predicate, all the particles are arranged in lexicographic order with a space delimiter
Consider the example sentence (8th sentence of neko.txt.cabocha) that "I saw human beings for the first time here." This sentence includes two verbs "begin" and "see", a phrase related to "starting" is "here", a phrase related to "seeing" is analyzed as "I am" and "one" The output should be as follows.

始める  で
見る    は を
Save the output of this program in a file and confirm the following items using the UNIX command.

Combination of frequent predicates and case patterns in corpus
Case pattern of verbs "do", "see" and "give" (order in descending order of occurrence frequency in corpus)
46. ​​Extraction of verb case frame information
Modify the program of 45 and output the term (the phrase itself pertaining to the predicate itself) in tab-delimited form following the predicate and case pattern. In addition to the specification of 45, it should satisfy the following specifications.

The term is a word string of the clause related to the predicate (there is no need to remove the last particle particle)
When there are plural clauses related to predicates, they are arranged in space and in the same standard and order as the particle
Consider the example sentence (8th sentence of neko.txt.cabocha) that "I saw human beings for the first time here." This sentence includes two verbs "begin" and "see", a phrase related to "starting" is "here", a phrase related to "seeing" is analyzed as "I am" and "one" The output should be as follows.

始める  で      ここで
見る    は を   吾輩は ものを
47. Mining of functional verb syntax
I want to pay attention only when there is a social change noun in the verb 's won case. Change the program of 46 to satisfy the following specifications.

Target only when the phrase constituted by "social change connection noun + with (particle)" relates to verb
Predicate is "Saga connection noun + is the basic form of verb", and when there are multiple verbs in a phrase, the leftmost verb is used
When there are two or more particles (phrases) related to a predicate, all the particles are arranged in lexicographic order with a space delimiter
When there are two or more clauses related to a predicate, arrange all the terms in a space delimited (align them in the order of particles)
For example, the following output should be obtained from the sentence "It will not go oversteps and the master will reply to the letter."

返事をする      と に は        及ばんさと 手紙に 主人は
Save the output of this program in a file and confirm the following items using the UNIX command.

Predicates frequently occurring in corpus (social change connection noun + with + verb)
Frequent predicates and particle patterns in the corpus
48. Extraction of path from noun to root
For a phrase containing all nouns in the sentence, extract the path from that phrase to the root of the syntax tree. However, the path on the syntax tree shall satisfy the following specifications.

Each phrase is represented by a morpheme string (surface layer type)
Link the representation of each phrase " ->" " from the start phrase of the path to the end phrase
From the sentence "I saw human beings for the first time here" (8th sentence of neko.txt.cabocha), the following output should be obtained.

吾輩は -> 見た
ここで -> 始めて -> 人間という -> ものを -> 見た
人間という -> ものを -> 見た
ものを -> 見た
49. Extraction of dependency path between nouns
Extract the shortest dependency path connecting all pairs of noun phrases in the sentence. However, if the clause number of the noun phrase pair is iAnd j( I < j), The dependency path shall satisfy the following specifications.

As in Problem 48, the path is ->expressed by concatenating expressions (surface morpheme strings) of each phrase from the start phrase to the ending phrase with " "
Clause iAnd jReplace noun phrases contained in
In addition, the following two possible shapes of the dependency path are conceivable.

Clause iClause on the path leading to the syntax tree roots from jIs present: clause iTo clause jShow path of
Other than the above, clause iAnd clause jA common phrase on the route leading to the syntax tree roots from kWhen intersecting with: clause iFrom phrase kThe path and the clause j just before reachingFrom phrase kThe path up to just before reaching, phrase kContents of " |" are concatenated and displayed
For example, the following output should be obtained from the sentence "8th sentence of neko.txt.cabocha" "I saw human beings for the first time here."

Xは | Yで -> 始めて -> 人間という -> ものを | 見た
Xは | Yという -> ものを | 見た
Xは | Yを | 見た
Xで -> 始めて -> Y
Xで -> 始めて -> 人間という -> Y
Xという -> Y
Chapter 6: Processing English Text
For the English text ( nlp.txt ), perform the following processing.

50. Sentence break
(. or; ​​or: or? or!) → Blank letters → Upper case letters as a sentence delimiter and output the entered documents in the form of one line per sentence.

51. Word segmentation
Consider the space as a delimiter of a word, accept the output of 50 as an input, and output it in the form of one word per word. However, output a blank line at the end of the sentence.

52. Stemming
51 output as input, apply Porter's stemming algorithm and output word and stem in tab-delimited format. In Python, as the implementation of the stemming algorithm Porter stemming may utilize modules.

53. Tokenization
Using Stanford Core NLP , obtain the analysis result of input text in XML format. Also, read this XML file and output the input text in the form of 1 line by 1 word.

54. Part of speech tagging
Read the analysis result XML of Stanford Core NLP and output words, renderers, and parts of speech in tab-delimited format.

55. Named entity extraction
Pull out all person names in the input sentences.

56. Co-reference analysis
Based on the result of co-reference analysis of Stanford Core NLP, replace the reference in the sentence with a representative reference. However, when replacing, take care so that the original reference expression can be understood, such as "representative reference expression (reference expression)".

57. Dependency analysis
Visualize the result (collapsed-dependencies) of the dependency analysis of Stanford Core NLP as a directed graph. The visualization, the dependency tree DOT language converted into, Graphviz preferably used. You can also use pydot to directly visualize a directed graph from Python .

58. Extraction of tuples
Based on the result of the dependency analysis of Stanford Core NLP (collapsed-dependencies), output the set of "subject predicate object" in tab-delimited format. However, please refer to the following for definition of subject, predicate, object.

Predicates: words with dependencies of nsubj relationships and dobj relationships
Subject: dependent from predicate to nsubj relation
Object: Dependent from dojj relationship from predicate
59. Analysis of S-expression
Read Stanford Core NLP phrase structure analysis result (S expression) and display all noun phrases (NP) in the sentence. Also display all nesting noun phrases.

Chapter 7: Databases
artist.json.gz is an open music database MusicBrainz that converts things related to artists into JSON format and compresses them in gzip format. In this file, information on one artist is stored in a single line in JSON format. The outline of the JSON format is as follows.

field	Type	Contents	An example
id	Unique identifier	integer	20660
gid	Global identifier	String	"ecf 9 f 3 a 3 - 35 e 9 - 4 c 58 - acaa - e 707 fba 45060"
name	artist name	String	"Oasis"
sort_name	Artist name (for dictionary ordering)	String	"Oasis"
area	Activity location	String	"United Kingdom"
aliases	alias	List of dictionary objects	
aliases []. name	alias	String	"oasis"
aliases []. sort_name	Alias ​​(for alignment)	String	"oasis"
begin	Activity start date	dictionary	
begin.year	Year of commencement	integer	1991
begin.month	Activity start month	integer	
begin.date	Activity start date	integer	
end	Activity end date	dictionary	
end.year	End of activity year	integer	2009
end.month	Activity end month	integer	8
end.date	Activity end date	integer	28
tags	tag	List of dictionary objects	
tags []. count	Tagged times	integer	1
tags []. value	Tag content	String	"rock"
rating	Rating	Dictionary object	
rating.count	Number of ratings votes	integer	13
rating.value	Rating value (average value)	integer	86
Consider storing and retrieving data of artist.json.gz in key-value-store (KVS) and document-oriented database. As KVS, use LevelDB , Redis , KyotoCabinet, etc. MongoDB was adopted as a document-oriented database, but CouchDB , RethinkDB, etc. may be used.

60. Construction of KVS
Use a key-value-store (KVS) and build a database to search for the activity location (area) from the artist name (name).

61. Search for KVS
Using the database constructed in 60, obtain the activity location of a specific (specified) artist.

62. Iterative processing in KVS
Find the number of artists whose activity location is "Japan" using the database constructed in 60.

63. KVS that stores object in value
Using KVS, build a database to search the list of tags and tag counts (tagged times) from the artist name (name). In addition, search the tag and the number of tags to be tagged from the artist name using the database constructed here.

64. Construction of MongoDB
Register artist information (artist.json.gz) in the database. In addition create indexes in the following fields: name, aliases.name, tags.value, rating.value

65. Search for MongoDB
Using MongoDB's interactive shell, get information on the artist "Queen". Furthermore, implement a program that performs the same processing as this.

66. Acquisition of number of searches
Find the number of artists whose activity location is "Japan" using MongoDB's interactive shell.

67. Acquiring multiple documents
Search artists with specific (specified) aliases.

68. Sort
Seek artist / top 10 with more ratings votes among artists who are tagged as "dance".

69. Creating a web application
Create a Web application that displays information on artists matching search criteria entered by users. Specify search conditions with artist name, artist's alias, tag, etc, and display the list of artist information in order of highest rating etc.

Chapter 8: Machine Learning
In this chapter, we use the sentence polarity dataset v1.0 of Movie Review Data published by Bo Pang and Lillian Lee to a task (polarity analysis) to classify sentences as positive (positive) or negative (negative) To tackle.

70. Acquisition and format of data
Using correct answer data for polar analysis on sentences , create correct answer data (sentiment.txt) in the following way.

Add a character string "+1" to the beginning of each line of rt-polarity.pos (the polarity label "+1" followed by the space followed by the contents of the positive sentence)
Add a character string "-1" to the beginning of each line of rt-polarity.neg (Polarity label "-1" followed by space followed by negative sentence contents)
Combine (concatenate) the contents of 1 and 2 above and rearrange the rows randomly
After creating sentiment.txt, check the number of positive examples (positive sentences) and the number of negative examples (negative sentences).

71. Stop word
Properly create a list (stop list) of English stopwords. In addition, implement a function that returns true if the word (character string) given as an argument is included in the stop list, and false otherwise. In addition write a test for that function.

72. Feature extraction
Design your own features that might be useful for polar analysis and extract features from training data. As a feature, removing the stop word from the review and stemming each word will be the minimum baseline.

73. Learning
Learn the logistic regression model using features extracted in 72.

74. Forecast
Using a logistic regression model learned in 73, implement a polarity label ("+1" for positive cases, "-1" for negative cases) and a program to calculate their prediction probabilities.

75. Weight of identity
In the logistic regression model learned in 73, check top 10 with high weight and top 10 with low weight.

76. Labeling
Apply a logistic regression model to the learning data, and output the label of correct answer, predicted label, prediction probability in tab delimited format.

77. Measurement of correct answer rate
76, and prepare a program that obtains the correct answer rate of the forecast, the relevance rate on the positive case, the recall rate, and the F1 score.

78. 5-way cross validation
In the experiment of 76-77, we used case for learning also for evaluation, so it can not be said that it is legitimate evaluation. In other words, the classifier evaluates the performance when memorizing training cases roundly, and does not measure the generalization performance of the model. Then, calculate the correct answer rate, relevance rate, recall rate, and F1 score for polarity classification by 5-way cross validation test.

79. Rate of conformity - rendering recall rate graph
Draw the relevance ratio - recall rate graph by changing the threshold value of the classification of the logistic regression model.

Chapter 9: Vector Space Method (I)
enwiki-20150112-400-r10-105752.txt.bz2 randomly sampled 1/10 of articles of about 400 words or more among English Wikipedia articles as of January 12, 2015 105, 752 The text of the article is compressed in bzip 2 format. Using this text as a corpus, I want to learn vectors (distributed expressions) that represent meanings of words. In the first half of chapter 9, the principal component analysis is applied to the word context co-occurrence matrix created from the corpus, and the process of learning the word vector is divided into several processes and implemented. In the second half of chapter 9, we calculate word similarity and analogy (analogy) using word vector (300 dimensions) obtained by learning.

If problem 83 is implemented obediently, a large amount (about 7 GB) of main memory is required. If the memory is insufficient, devise the process or use the 1/100 sampling corpus enwiki - 20150112 - 400 - r100 - 10576.txt.bz 2 .

80. Corpus formatting
The simplest way to convert a sentence to a word string is to break it into words with whitespace. However, in this method, words are included in the words such as period endings and parentheses. Therefore, after dividing the text of each line of the corpus into a list of tokens with blank characters, apply the following processing to each token and remove the symbol from the word.

Delete the next occurrence of characters at the beginning and end of the token: .,!?;:()[]'"
Delete tokens that are empty string
After applying the above process, save the token in a file by concatenating it with a space.

81. Dealing with a country name composed of compound words
In English, articulation of multiple words may make sense. For example, the United States is expressed as "United States" and the United Kingdom as "United Kingdom" but with the words "United", "States" and "Kingdom" the concepts and entities being indicated are ambiguous. Therefore, we want to estimate the meaning of compound words by recognizing compound words contained in corpus and handling compound words as one word. However, it is very difficult to accurately certify compound words, so here we want to recognize the country name consisting of compound words.

Acquire the list of countries from the Internet on their own, replace the space with underscores for the country names of compound words appearing in the 80 corpus. For example, "United States" should be "United_States", "Isle of Man" should be "Isle_of_Man".

82. Extract context
All the words t appearing in the corpus created in 81, The word tAnd the context word cPlease write out all pairs in tab delimited format. However, the definition of the context word is as follows.

A word tBefore and after dThe word is defined as context word c(Except that the word tIt does not include it)
The word tEvery time you choose, the context width dIs { 1 , 2 , 3 , 4 , 5 }Within the range of.
83. Measurement of Word / Context Frequency
Using the output of 82, find the following appearance distribution and constant.

f( t , c ): Word tAnd the context word cCo-occurrence frequency
f( t , * ): Word tNumber of occurrences
f( * , C ): Context word cNumber of occurrences
N: Total number of occurrences of word and context word pair
84. Creating a word context matrix
Using the output of 83, the word context matrix XMake it. However, the matrix XOf each element Xt cIs defined as follows.

f( t , c ) ≥ 10Then, Xt c= P P M I ( t , c ) = max { logN× f( t , c )f( t , * ) * f( * , C ), 0 }
f( t , c ) < 10Then, Xt c= 0
Here, P P M I ( t , c )Is a statistic called Positive Pointwise Mutual Information (positive mutual information). The matrix XThe number of rows and the number of columns will be in the order of several million and it is impossible to place all the elements of the matrix on the main memory. Fortunately, the matrix XMost of the elements are 0Therefore, non- 0You can write only elements of.

85. Dimensional compression by principal component analysis
Apply principal component analysis to the word context matrix obtained in 84 and compress the semantic vector of the word to 300 dimensions.

86. Display of word vector
Read the semantic vector of the word obtained in 85 and display the vector "United States". Note, however, that "United States" is internally represented as "United_States".

87. Word similarity
Read the semantic vector of the word obtained in 85 and calculate the cosine similarity between "United States" and "US". However, note that "US" is internally expressed as "US".

88. 10 words with high similarity
Read the semantic vector of the word obtained in 85, output 10 words with high cosine similarity to "England" and its similarity.

89. Analogy based on additive constructivity
Read the semantic vector of the word obtained in 85, calculate vec ("Spain") - vec ("Madrid") + vec ("Athens"), output 10 words with high similarity and its similarity Do it.

Chapter 10: Vector Space Method (II)
In chapter 10, we will continue to learn word vectors as in the previous chapter.

90. Learning with word2vec
Apply word2vec to the corpus created in 81 and learn the word vector. Furthermore, convert the form of the learned word vector and move the program of 86-89.

91. Preparation of analogy data
Download the word analogy evaluation data . The line beginning with ":" in this data represents the section name. For example, the line ": capital-common-countries" represents the beginning of the section "capital-common-countries". In the downloaded evaluation data, extract the evaluation case included in the "family" section and save it in a file.

92. Application to analogy data
Vec (word in the second row) - vec (word in the third row) + vec (word in the third row) is calculated for each case of the evaluation data created in 91, and the similarity with that vector is the most similar Find a high word and its similarity. Add the word and similarity to the end of each case. Apply this program to the word vector created in 85, the word vector created in 90.

93. Calculation of correct answer rate of analogy task
Using the data created in 92, find the correct rate of analogy task of each model.

94. Similarity calculation in WordSimilarity-353
The WordSimilarity - 353 Create a program to input the evaluation data of the Test Collection , calculate the similarity between words in the first and second columns, and add the value of similarity to the end of each line. Apply this program to the word vector created in 85, the word vector created in 90.

95. Evaluation with WordSimilarity-353
Calculate the Spearman correlation coefficient between the ranking of similarity output by each model and the ranking of human similarity judgment using the data created in 94.

96. Extraction of vector on country name
From vector 2vec's learning result, extract only the vector concerning the country name.

97. k-means clustering
For 96 word vectors, k-means clustering is divided into cluster number k = 5Run as.

98. Clustering by Ward's method
For 96 word vectors, perform hierarchical clustering by the Ward method. Furthermore, visualize the clustering result as a dendrogram.

99. Visualization by t-SNE
For 96 word vectors, visualize the vector space with t - SNE.
