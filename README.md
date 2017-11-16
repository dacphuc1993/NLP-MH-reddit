# NLP-MH-reddit
This is the code for my thesis research. The `mh_reddit.ipynb` file does the following: 
- Import data in JSON format (`post_2014.json`, `comment_2014.json`) into a Python list of dictionaries.
- Construct users classes: MH and MH->SW.
- Construct sets of features from posts and comments: sentiment, content, interpersonal, linguistic, metadata/interaction, full (combination of all 4 sets).
- Carry out z-test for 2 populations: MH and MH->SW.
- Write sets of features to CSV file.

The `classification.ipynb` uses sets of features above to classify between MH users and MH->SW users as a supervised learning task.
There are 3 classifiers in this task: SVM, Naive Bayes and Logistic regression.

The experiment has 2 settings: theoretical setting (465 MH vs 465 MH->SW) and realistic setting (247614 MH vs 465 MH->SW)

The CSV files with "_2" suffix indicates features of realistic setting.
