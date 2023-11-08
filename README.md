# NLP_StockPrediction (based-on-News-Headlines)

Stock often fluctuates based on the news headline. Briefly, evaluating the diversity of news headlines can provide valuable insights into the stock market's future. So, here sentiment of stock has been analyzed to predict a fall or rise in near future only using news paper headlines.


# Workflow

* Collected Dataset from Kaggle 
* Preprocessed using NLTK
* Used CountVectorizer for word embedding
* Implemented Classifiers are - Random Forest & Naive Bayes
* Confusion matrices are generated to visualize and summarize the performance of all the classification algorithms
  
# A random forest classifier.
A random forest is a meta estimator that fits a number of decision tree classifiers on various sub-samples of the dataset and uses averaging to improve the predictive accuracy and control over-fitting. The sub-sample size is controlled with the max_samples parameter if bootstrap=True (default), otherwise the whole dataset is used to build each tree.
Random Subsampling (Bootstrap Aggregating or Bagging): Random Forest creates multiple subsets of the training data by sampling with replacement. Each subset is used to train a different decision tree. This helps reduce overfitting and improves model robustness.
Random Feature Selection: At each split in the tree, a random subset of features is considered for splitting, not the entire set of features. This introduces diversity and reduces the correlation among trees.

# Bag of Words Model (BoW):
The Bag of Words model is a popular text representation technique used in natural language processing. It represents text data as a "bag" or "set" of words, ignoring the order and structure of the words in the text.
In the BoW model, a document is represented by a vector where each dimension corresponds to a unique word in the entire corpus, and the value in each dimension represents the frequency (count) of that word in the document.
BoW is widely used in tasks such as document classification, sentiment analysis, and text retrieval.

# Confusion matrix
Confusion matrix is a very popular measure used while solving classification problems. It can be applied to binary classification as well as for multiclass classification problems.
Confusion matrices represent counts from predicted and actual values. The output “TN” stands for True Negative which shows the number of negative examples classified accurately. Similarly, “TP” stands for True Positive which indicates the number of positive examples classified accurately. The term “FP” shows False Positive value, i.e., the number of actual negative examples classified as positive; and “FN” means a False Negative value which is the number of actual positive examples classified as negative. One of the most commonly used metrics while performing classification is accuracy. The accuracy of a model (through a confusion matrix) is calculated using the given formula below.

![image](https://github.com/Harshiths1/NLP_StockPrediction/assets/136854105/521e67d0-052b-4b4d-b9a9-ba6f8b85f98d)



