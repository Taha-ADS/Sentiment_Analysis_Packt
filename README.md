###  Sentiment Analysis on Airline Tweets**

This project performs sentiment analysis on real-world airline tweets to classify user opinions as positive or negative. It uses natural language processing (NLP) techniques and logistic regression to train a predictive model.

We compare two versions of the model:

* **Standard Logistic Regression**
* **Balanced Logistic Regression** (`class_weight='balanced'`) to address class imbalance

---

### 🚀 **Features**

* Loads and preprocesses tweet data
* TF-IDF vectorization of text
* Logistic regression classifier
* Evaluation using F1 score, AUC, confusion matrix, and classification report
* Visualization of model performance
* Detection of most confidently wrong predictions
* Interactive function to predict sentiment of custom text

---

### 📊 **Performance Comparison**

* **Without balancing**: May favor the majority class (e.g., negative reviews)
* **With `class_weight='balanced'`**: Improved fairness and recall for minority class (e.g., positive reviews)

---

### 📁 **Dataset**

* Source: Airline Tweets dataset from [LazyProgrammer.me](https://lazyprogrammer.me/course_files/AirlineTweets.csv)

---

### 🧠 **Technologies Used**

* Python
* scikit-learn
* pandas, NumPy
* seaborn & matplotlib
* TfidfVectorizer

---

### 📈 **Try It Out**

```python
predict_sentiment("The staff was super helpful and the flight was smooth.")
# Output: Positive (Confidence: 0.92)
```


