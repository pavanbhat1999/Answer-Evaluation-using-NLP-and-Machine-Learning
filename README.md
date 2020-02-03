# Answer-Evaluation-using-NLP-and-Machine-Learning
An experimental project based on Machine Learning and NLP for evaluation of answer scripts

### LOGIC and CONCEPT

 The theme of the project is to automate the process of evaluation of answer scripts of the student.
  (here are the screenshots regarding the project)

You can give your answer in the localhost and run Eval.py to get answer



### 1.Descriptive Answers
Firstly we collected answers from the Teachers and Resource persons and added that to the model answers Database.

As the system evaluates more and more paper it's model answers database gets updated regularly.


Evaluation is done based on following things

#### 1. Keywords
#### 2. Grammer
#### 3. Fuzzy logic Score for Ignorable mistakes
#### 4. Synonym checking 
#### 5. Sequence of statements (for some subjects)

Our ML will predict the quality of answers based on these things

Allotment of marks takes according to the quality of answers


##### 1. keywords

keywords are externaly provided and also extracted using data scraping and frequency distribution techniques.

Evaluation of Keywords based Cosine Similarity of "student answer" with "model answer".

Firstly texts (i.e. student's and model answer) converted into vectors. And from these two vectors the Cosine similarity is Calculated.

Now this gives value from 0 to 1. this is converted into numeric form (i.e. 0 to 100). And then keywords will get the value from 1-6


##### 2. Grammer

This is checked using certain online compilers thanks for that 

For this number of grammatical mistakes taken into consideration.

PS:TODO

##### 3. Ignorable Mistakes

Fuzzy Logic is used to give the value of Minimum editables

(You can find screenshots regarding that in the project)
(FuzzyWuzzy libraray from https://github.com/seatgeek/fuzzywuzzy this is used.




##### 4. Synonym Checking 

Python Libraries are used to get similer meaning words

You can even use pydictionary

that found new word is also added into the database of model answers.

##### 5. Sequence

certain questions need to be answered in certain sequences so that is also checked in our algo according to the model 

answers provided by assignong priority.









____________add Mathematics________________






For Any Suggestions please let me know here phinixbhat@gmail.com

