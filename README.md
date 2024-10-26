# Restaurant Recommendation System


This repository contains code for recommending restaurants based on user preferences. Developed using Flask and Python, the system leverages cosine similarity to suggest personalized dining options. The website is hosted on Python Anywhere, with the live app accessible at [Restaurant Rider](http://restaurantrider.pythonanywhere.com/).

## Project Overview

This project aims to provide users with customized restaurant recommendations by considering factors such as cuisine, budget, locality, and the number of people. The recommendation engine is developed with Scikit-learn’s cosine similarity functionality for NLP, while Flask enables a seamless web-based interface.

## Project Structure

```plaintext
.
├── app.py                  # Main application file
├── requirements.txt        # Dependencies
├── templates/              # HTML templates (home.html, search.html)
├── static/                 # Static files (CSS, JS)
├── food1.csv               # Dataset used for recommendations
└── README.md               # Project documentation
```

## Features

- **Customized Recommendations**: Based on user inputs for budget, locality, cuisine, and dining preferences.
- **Cosine Similarity**: Utilized to provide similar restaurant options using NLP.
- **Responsive Web Interface**: Built with Flask for seamless interaction.

## Getting Started

### Prerequisites
- Python 3.x
- Flask
- Scikit-learn
- Pandas
- Numpy

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Vigneshwar-B/Restaurant-Recommendation-System.git
   cd Restaurant-Recommendation-System
   ```

2. Set up a virtual environment:
   ```bash
   python3 -m venv env
   source env/bin/activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Application

1. Start the Flask application:
   ```bash
   flask run
   ```

2. Open a browser and navigate to `http://localhost:5000` to access the application.

## Used Technologies

- **Python**: Core programming language for backend development.
- **Flask**: Web framework for creating the RESTful service.
- **Scikit-learn**: Used for recommendation algorithms.
- **Pandas & Numpy**: Data manipulation and processing.
- **Gunicorn**: Production server for handling application requests.

## Project Workflow

### Recommendation Logic

The recommendation function `rest_rec` uses:
- **Locality** and **Cuisine Filters**: Filters based on user’s locality and cuisine preferences.
- **Cosine Similarity**: Computes similarity between restaurants based on highlights.
- **Budget Constraints**: Filters based on user-specified budget per person.

### Core Functions

- `fav()`: Uses cosine similarity to get a list of similar restaurants based on user preferences.
- `rest_rec()`: Filters restaurants based on user’s cost, locality, and cuisine preferences.
- `calc()`: Aggregates results from the above functions for display.

## Usage

1. **Homepage**: Enter details such as budget, cuisine, and locality.
2. **Search Results**: View restaurant recommendations tailored to the input criteria.
3. **Recommendation Method**: Utilizes cosine similarity to suggest top matches.

## Deployment

The application is hosted on Python Anywhere. For production use, configure environment variables and server settings according to your hosting service’s guidelines.

## How to Contribute

1. Fork the repository and create a new branch for your feature.
2. Make your modifications.
3. Submit a pull request with a summary of your changes.


### References <img src="https://www.flaticon.com/svg/static/icons/svg/1420/1420886.svg" width="24px">
#### For Building machine learning model and deployment:
1. https://medium.com/the-andela-way/deploying-a-python-flask-app-to-heroku-41250bda27d0
2. https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.cosine_similarity.html
3. https://www.machinelearningplus.com/nlp/cosine-similarity/
4. https://towardsdatascience.com/cosine-similarity-how-does-it-measure-the-similarity-maths-behind-and-usage-in-python-50ad30aad7db
5. https://uoa-eresearch.github.io/eresearch-cookbook/recipe/2014/11/26/python-virtual-env/
6. Machine Learning course- https://www.coursera.org/learn/machine-learning/

## Developer Details

- **Developer**: Vigneshwar B.
- **GitHub**: [Vigneshwar-B](https://github.com/Vigneshwar-B)
- **Contact**: vigneshbw2002@gmail.com



