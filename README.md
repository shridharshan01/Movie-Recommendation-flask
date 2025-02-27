# Movie Recommender System
This project is a Machine Learning-based Movie Recommender System designed to predict user ratings for movies using cosine similarity. The application leverages user preferences and historical data to provide personalized movie recommendations, enhancing the movie-watching experience.

# Features
- Personalized Recommendations: Utilizes cosine similarity to suggest movies based on user ratings and preferences.
- Rating Prediction: Predicts user ratings for unseen movies, helping users discover films they might enjoy.
- Interactive Web Interface: Built with Flask, providing a user-friendly experience for inputting preferences and viewing recommendations.
- Data Visualization: Visual representations of user preferences and movie ratings for better insights.

# Technologies Used
- Flask: A lightweight web framework for building the web application.
- Pandas: For data manipulation and analysis.
- NumPy: For numerical operations and calculations.
- Scikit-learn: For implementing machine learning algorithms, including cosine similarity.
- HTML/CSS/JavaScript: For front-end development and creating an interactive user interface.

# Code Snipets
Two of the following snippets of code were written to demonstrate the use of TFIDF and Cosine SImilarity in generating recommendations.

# Python Code
The python code in app.py will generate a list of movie recommendations provided that the user entered a valid movie name. When the entered movie name matches with a movie name in the dataset, recommendations will be generated according to the soup column (all details concatenated into one string) of each movie. In this set of code, the TF-IDF Vectorizer and Cosine Similarity function is imported from the “scikit-learn” package.
scikit-learn documentation: [TF-IDF vectoriser](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html?highlight=tfidf#sklearn.feature_extraction.text.TfidfVectorizer) and [Cosine Similarity](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.cosine_similarity.html#sklearn.metrics.pairwise.cosine_similarity)

# Javascript Code
The javascript code in notfound.html is executed when the user entered an invalid movie name. This set of code will return movie titles that are similar to the input that the user has entered, if applicable. The entered data will be checked against all existing movie names to find the most similar movie names. Since this snippet of code doesn't use any packages, a dictionary was created to store the terms for vectorising purposes and several functions were also created to compute the TF-IDF and Cosine Similarity values.

![Screenshot 2025-02-27 185436](https://github.com/user-attachments/assets/7ab8cce0-cc70-4e72-9e25-525c1396a124)

![Screenshot 2025-02-27 190026](https://github.com/user-attachments/assets/bbcb6ef1-11b2-4014-ad48-cdae5182d50f)

![Screenshot 2025-02-27 185329](https://github.com/user-attachments/assets/b493e7cf-df96-430c-84ba-d2601b537dc4)

# Setup
1. Install the required packages:
```bash
  pip install -r requirements.txt
```
2. Run the application:
```bash
  python app.py
```

