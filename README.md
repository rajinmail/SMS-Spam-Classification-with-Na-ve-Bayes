# SMS Spam Classification with Naïve Bayes

## Overview
This Python script demonstrates the use of a Naïve Bayes classifier to classify SMS messages as spam or ham (non-spam). The script uses the SMS Spam Collection dataset, where each message is labeled as either 'spam' or 'ham'. It preprocesses the data, splits it into training and testing sets, converts the text messages into a frequency matrix using CountVectorizer, and trains a Multinomial Naïve Bayes classifier. The accuracy of the classifier is then evaluated on the testing set.

## Prerequisites
Make sure you have the required libraries installed. You can install them using the following command:

```bash
pip install pandas scikit-learn
```

## Usage
1. Clone the repository:

```bash
git clone https://github.com/rajinmail/sms-spam-classification.git
cd sms-spam-classification
```

2. Download the [SMS Spam Collection dataset](https://archive.ics.uci.edu/ml/datasets/sms+spam+collection) and save it as 'SMSSpamCollection' in the project directory.

3. Run the script:

```bash
python sms_spam_classification.py
```

## Code Description
- **Load SMS Data:**
  - Loads the SMS Spam Collection dataset into a Pandas DataFrame.

- **Convert Labels to Binary Values:**
  - Maps 'ham' to 0 and 'spam' to 1 for binary classification.

- **Split Data into Training and Test Sets:**
  - Splits the data into training and testing sets using `train_test_split`.

- **Transform Data into Occurrences:**
  - Uses `CountVectorizer` to convert text messages into a frequency matrix.

- **Build Naïve Bayes Classifier:**
  - Creates and trains a Multinomial Naïve Bayes classifier using `MultinomialNB`.

- **Evaluate Classifier:**
  - Uses the trained classifier to make predictions on the testing set and calculates accuracy.

- **Display Dataset Information:**
  - Prints the original dataset size, the number of messages in the training set, and the number of messages in the testing set.

## Results
The script outputs the accuracy of the Naïve Bayes classifier on the testing set, providing an assessment of the model's performance in classifying SMS messages as spam or ham.

Feel free to explore additional metrics, modify parameters, or experiment with different classifiers for further analysis.
