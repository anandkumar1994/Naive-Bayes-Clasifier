
OBJECTIVE:
The target of task is 
•	To build up a Multi-Value Classification pipeline 
•	To characterize content into various marks. 
•	The information will be content, given as a string, and the yield must be a rundown of marks coordinating the classes of the given content. 
•	The corpus is the Reuters corpus from NLTK. To assess, utilize diverse measurements and give an account of their quality.

CLASSIFIER USED IN TASK:
	Support Vector Classifier and Linear Support Vector Classifier are used as a classifier to characterize content in to various marks and it is used to increase the accuracy, precision, recall for the given corpus (Reuters).

USES OF SVC CLASSIFIER IN ASSIGNMENT:
•	It is simple and quick to foresee class of test informational index. It additionally perform well in multi class forecast 
•	Compelling in high dimensional spaces. 
•	Still compelling in situations where number of measurements is more noteworthy than the quantity of tests. 
•	Utilizations a subset of preparing focuses in the choice capacity (called support vector), so it is likewise memory productive. 
•	Flexible: distinctive Kernel capacities can be indicated for the choice capacity. Regular parts are given, yet it is likewise conceivable to indicate custom bits.

DOWNLOADED PACKAGES:
This command `nltk.download ('all') downloads all packages. The used packages in the tasks are
•	Reuters  
•	Punkt
•	Stopwords
•	WordNet

TO INCREASE THE ACCURACY, PRECISION, RECALL:
STEP 1: REMOVING SPECIAL CHARACTERS & NUMBERS USING REGEX CONCEPT
To enhance the accuracy is by evacuating special characters .We can evacuate the special characters by utilizing regex. The regex we utilized as a part of the code is 
re.match ("[a-zA-Z]+”)]. It will matches with every one of the strings that begin with letters. By along these lines we can evacuate the unique characters and can enhance the precision.
STEP 2:  STEMMING
Stemming and Lemmatization are other two highlights we can use to expel the rehashed words like feline and felines which gives both same significance , when we attempt to discover the data from the recurrence of N words , words may rehash which involves more memory . So to defeat this issue we can utilize either stemming or lemmatization. 
Stemming as a rule introduces to a rough heuristic process that hacks off the closures of words in the expectation of accomplishing this objective accurately more often than not, and regularly incorporates the expulsion of derivational joins. 
The disadvantage of lemmatization is it isn't precise contrast with the stemming. Likewise for lemmatization, we need to utilize every one of the parts of speech and different libraries which make the code jumbled. Keeping in mind the end goal to enhance the exactness we are utilizing stemming.
STEP 3: REMOVING STOPWORDS
Stop words are only an arrangement of usually utilized words in any dialect. Stop words are generally removed from numerous content preparing applications. In light of the fact that these words can be diverting, non-educational (or non-discriminative) and are extra memory overhead. 
By dispensing with stop words 
•	We can enhance the intensity of forecast
•	We can build the memory. 
•	We can diminish false positives. 

FEATURE EXTRACTION:
Make Training and testing set. Each article will be changed to an element vector of 0 and 1, If the record contains the chose highlight word or not. It begins from an underlying arrangement of estimated information and manufactures determined qualities (highlights) proposed to be instructive and non-repetitive, encouraging the ensuing learning and speculation steps, and now and again prompting better human elucidations

CLASSIFIER TRAINING USING SVC, LINEAR SVC:	
            Support vector classification (SVC) is a set of supervised learning methods used for classification, regression and outlier’s detection. The implementation is based on libsvm. The multiclass support is handled according to a one-vs-one scheme. SVC and NuSVC are similar methods, but accept slightly different sets of parameters and have different mathematical formulations. 
            LinearSVC (one-vs-the-rest scheme) is another implementation of Support Vector Classification for the case of a linear kernel. The implementation is based on liblinear Note that LinearSVC does not accept keyword kernel, as this is assumed to be linear. It also lacks some of the members of SVC and NuSVC, like support. This class supports both dense and sparse input and the multiclass support is handled according to a one-vs-the-rest scheme.

ACCURACY, PRECISION, RECALL OBTAINED USING SVC:
From the given corpus I had attempted to evacuate the stop words, extraordinary characters, 
Numbers with the assistance of normal articulation. Likewise, I have acquainted the idea of 
Stemming with additionally increment the precision to up to 62.11%. At last, the exactness,
 Review and F1-score that I have accomplished are as per the following:

Accuracy: 0.6211
Precision: 0.2524
Recall   : 0.1389
F1-Score: 0.1646

