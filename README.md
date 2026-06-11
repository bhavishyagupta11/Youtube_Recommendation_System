# Deep YouTube Recommendations

![Python Version](https://img.shields.io/badge/python-3.x-blue.svg)
[![Version](https://img.shields.io/badge/version-v1.0.0-orange)](https://github.com/bhavishyagupta11/Youtube_Recommendation_System)
![GitHub repo size](https://img.shields.io/github/repo-size/bhavishyagupta11/Youtube_Recommendation_System)

An implementation of the recommender systems for **YouTube** as described in the paper: [Deep Neural Networks for YouTube Recommendations](https://static.googleusercontent.com/media/research.google.com/ko//pubs/archive/45530.pdf).

This project focuses on providing an end-to-end framework, starting from data processing to model training and ranking, utilizing Deep Learning techniques to generate candidate recommendations and rank them effectively.

## 🚀 Features

- **Candidate Generation**: A deep neural network architecture designed to retrieve a small subset of videos (hundreds) from a massive corpus, using user history and context.
- **Ranking Model**: A fine-grained ranking model to score the generated candidates, maximizing expected user engagement.
- **MovieLens Integration**: Out-of-the-box support for the [MovieLens](https://grouplens.org/datasets/movielens/) dataset to train and test the recommendation engine.

## ⚙️ Development Environment

- **Language**: Python 3.x
- **Framework**: TensorFlow 2.x

## 💻 Usage

To run the model training process, simply execute the training script:

```bash
python train.py
```

## 🧠 Model Architecture

The recommendation system consists of two primary stages, mirroring the architecture from the original Google paper:

### 1. Candidate Generation
This stage uses the user's activity history to pull a small subset of candidate videos from a much larger corpus. It acts as a coarse filter to quickly narrow down options.

<img width="773" alt="Candidate Generation Architecture" src="https://user-images.githubusercontent.com/21326503/92299725-fd76bb00-ef8f-11ea-82c3-a1e6a15f65ad.png">

### 2. Ranking
The generated candidates are then fed into a highly parameterized ranking model, which provides a fine-grained score for each item, typically optimizing for user engagement metrics like watch time.

<img width="773" alt="Ranking Architecture" src="https://user-images.githubusercontent.com/21326503/92299764-60685200-ef90-11ea-8389-2fa514124aae.png">

## 👨‍💻 Developer

- **Bhavishya Gupta**

## 📚 References

- **Paper**: [Deep Neural Networks for YouTube Recommendations](https://static.googleusercontent.com/media/research.google.com/ko//pubs/archive/45530.pdf)
- **Dataset**: [MovieLens](https://grouplens.org/datasets/movielens/)
