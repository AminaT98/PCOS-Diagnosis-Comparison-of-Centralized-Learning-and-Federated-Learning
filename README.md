# PCOS-Diagnosis-Comparison-of-Centralized-Learning-and-Federated-Learning
Diagnosis of PCOS using Centralized vs. Federated Learning. Trained models on the same dataset using both approaches to compare accuracy, privacy, and performance. Federated setup simulated with Flower across virtual clients. Focus: evaluating FL's potential in sensitive healthcare contexts.

This project explores the use of Federated Learning (FL) in the early detection of Polycystic Ovary Syndrome (PCOS) while prioritizing data privacy and distributed collaboration. The approach simulates a real-world healthcare scenario where patient data is stored across multiple institutions and cannot be centralized due to confidentiality constraints.

The work is divided into two main stages:

1. Centralized Baseline Model
As a first step, I trained a machine learning model using a centralized version of the dataset from Kaggle. This phase helped define a baseline for accuracy and model behavior using traditional data processing techniques.

2. Federated Learning Simulation
The second phase involved implementing a federated architecture using Flower, an open-source FL framework. Here, the dataset was split into multiple virtual clients, each simulating a separate data-holding institution. Each client trained locally, and only model updates were shared with the server for aggregation—no raw data left the device.

=> I used:

- Python for data preprocessing, model design, and orchestration
- scikit-learn for building and evaluating the ML models
- Flower to manage the FL workflow and simulate client-server interactions
- Matplotlib & Seaborn for result visualization and comparison

=> Key Goals:
- Ensure privacy-first learning without centralizing sensitive health data
- Compare model performance between centralized and federated approaches
- Explore how FL can support healthcare decision-making in low-resource or distributed environments

=> Outcome:
The federated setup achieved comparable accuracy to the centralized model while maintaining strict data separation. This experiment supports the idea that federated learning can be a viable and ethical solution for real-world medical applications—especially in contexts where data privacy, regulation, and decentralization are non-negotiable.
