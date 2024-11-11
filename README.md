# 📰 Fake News Detection Project

## Overview
This project focuses on detecting fake news using machine learning models like **Logistic Regression** and **Decision Tree Classifier**. It uses the [Fake and Real News Dataset](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset) from Kaggle to train and evaluate the models.

The main goal of this project is to classify news articles into **Fake News** or **True News** using natural language processing (NLP) and machine learning techniques. The project demonstrates the end-to-end process of loading data, cleaning it, training ML models, and evaluating the results. 🤖✨

## 📂 Dataset
The dataset consists of two CSV files: **Fake.csv** and **True.csv**. Both files contain articles labeled as fake or real news.

- **Columns**: `title`, `subject`, `date`, `text`
- The `title`, `subject`, and `date` columns were dropped to focus solely on the `text` column for our analysis.

## 🛠️ Libraries Used
- `pandas` for data manipulation
- `numpy` for numerical operations
- `matplotlib` & `seaborn` for visualization
- `scikit-learn` for machine learning and data preprocessing
- `re` and `string` for text cleaning

## 🧹 Data Preprocessing
The `wordopt` function is used to clean the text by:
- Converting to lowercase 🐍
- Removing punctuation and special characters ✂️
- Removing URLs and HTML tags 🌐
- Removing words with digits 🔢

## 📊 Machine Learning Models
Two machine learning models were used:

1. **Logistic Regression**
   - Achieved an accuracy of **98.67%** on the test set.
2. **Decision Tree Classifier**
   - Achieved an accuracy of **99.63%** on the test set.

The evaluation metrics used include **precision**, **recall**, and **f1-score**. The results demonstrate strong performance for both models. 📈💯

## 🖥️ Model Predictions
A custom function called `manual_testing` allows the user to input a piece of news and get predictions from both models:

```python
def manual_testing(news):
    # Predict whether the news is Fake or True
    LR Prediction: "True News" or "Fake News"
    DT Prediction: "True News" or "Fake News"
```

## 🚀 How to Run the Project
1. Clone this repository:
   ```sh
   git clone https://github.com/usmanumar97/fake-news-detector.git
   ```
2. Install the required libraries:
   ```sh
   pip install -r requirements.txt
   ```
3. Run the script to train and test models.
4. Use the `manual_testing(news)` function to classify your own news articles!

## 🤖 Future Improvements
- Adding more sophisticated models like **Random Forest** or **SVM**.
- Implementing **Ensemble Learning** for better prediction accuracy.
- Creating a web app using **Streamlit** to make the classifier more accessible.

## 🤝 Contributing
Feel free to fork this repository and submit pull requests. Any contributions to make this project better are welcome! 😄✨

## 📄 License
This project is licensed under the MIT License.

## 📧 Contact
If you have any questions, reach out at [usmanumar92@gmail.com](mailto:usmanumar92@gmail.com).

Happy coding! 🚀

