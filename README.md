# Clickbait Headline Detection

This project is a data science exploration into detecting clickbait headlines. It uses a combination of classic machine learning and deep learning models to classify headlines as either clickbait or not.

This isn't a super serious, "change the world" kind of project. It was more of a fun exercise to play with different NLP techniques and see how well I could build a classifier. I'm sharing it in the hope that it might be useful to someone else who is learning data science.

## What's Inside

This repository contains:

- **Jupyter Notebooks**: The core of the project, showing the step-by-step process from data exploration to model building.
- **Data**: The dataset used for training and testing the models.
- **Saved Models**: The trained models are saved so you can easily use them.

## The Dataset

The data is split into two files: `train1.csv` and `train2.csv`. It's a simple dataset with two columns: `headline` and `clickbait` (1 for clickbait, 0 for not).

I didn't create this dataset myself, but it's a pretty standard one for this kind of task.

## How It's Organized

The project is structured as follows:

```
├── data/
│   ├── train1.csv
│   └── train2.csv
├── models/
│   ├── 01_EDA.ipynb
│   ├── 02_Classic_ML.ipynb
│   ├── 03_Deep_Learning.ipynb
│   └── requirements.txt
├── LICENSE
└── requirements.txt
```

- `data/`: Contains the raw data.
- `models/`: This is where the magic happens. It has the notebooks for EDA, classic machine learning, and deep learning.
- `requirements.txt`: The main dependencies for the project.

## Getting Started

If you want to run this project on your own machine, here's what you need to do:

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/Click_Bait-Detection-Model.git
    ```

2.  **Create a virtual environment (recommended):**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

    There's also a `requirements.txt` in the `models` folder. They are identical, so you only need to install one.

4.  **Run the notebooks:**
    Open Jupyter Notebook and navigate to the `models` directory. You can then run the notebooks in order:
    - `01_EDA.ipynb`: To see the data analysis.
    - `02_Classic_ML.ipynb`: To train and evaluate the classic machine learning models.
    - `03_Deep_Learning.ipynb`: To train and evaluate the deep learning model.

## The Models

I've experimented with a few different models:

- **Logistic Regression**: A simple and effective baseline model.
- **Naive Bayes**: Another classic model that works well for text classification.
- **LSTM (Long Short-Term Memory)**: A deep learning model that can capture the sequence of words in a headline.

The notebooks go into more detail about how these models were built and evaluated. The trained models are saved in the `models/` directory using `joblib`.

## A Few Last Words

This was a learning project for me. It's not perfect, but it's a good starting point for anyone interested in NLP and clickbait detection. Feel free to fork it, play with it, and let me know if you have any suggestions!
