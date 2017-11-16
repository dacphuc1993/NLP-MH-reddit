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

The TXT files `token.txt` and `token_2.txt` are the same in content, but one contains underscore "_" in bigrams and the others does not. 

The `post_2014.json` and `comment_2014.json` are large (more than 500MB), so I uploaded them [here](https://drive.google.com/open?id=1r2aDjfmsXkWNkf77iO40VMJ6Uu1zbPdn) and [here](https://drive.google.com/open?id=1eSqj4pVvvnSxjTURdKFA0OGqA5QYDbNf).

The PDF version of my thesis can be found [here](https://drive.google.com/open?id=1wTC4P1e0EWOnB2EVihfcokPA_7Wo_x2d).

The Latex code for my thesis can be found [here](https://github.com/dacphuc1993/master-thesis).
