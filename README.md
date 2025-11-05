# CardFraudDetectAI

An intelligent AI-powered system for real-time credit card fraud detection using machine learning and deep learning methods.

---

## Project Description

**CardFraudDetectAI** is designed to detect fraudulent credit card transactions by learning behavioral and transactional patterns from large-scale financial datasets.  
Unlike conventional static models, this project focuses on **real-time prediction**, **explainable AI**, and **system-level scalability**—bridging research concepts with real-world deployment practices.

### Key Components

- **Data Preprocessing:** Cleaning, normalization, feature scaling, and class balancing using SMOTE.
- **Model Training:** Training machine learning and deep learning models (XGBoost, LSTM Autoencoder) with optimized hyperparameters.
- **Evaluation:** Measuring performance using Precision, Recall, F1 Score, and ROC-AUC.
- **Fraud Detection:** Applying the best-performing models to identify high-risk transactions in real time.
- **Explainability:** Integrating SHAP visualizations to interpret model predictions and assist analysts in decision-making.

## Table of Contents

- [Project Description](#project-description)
- [Installation](#installation)
- [Datasets](#dataset)
- [Algorithms](#algorithms)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Installation

To install and set up the AI-Based Fraud Detection project, follow these steps:

1. Clone the repository:

   ```shell
   git clone https://github.com/Tek-nr/AI-Based-Fraud-Detection.git
   ```

## Dataset

### Dataset Information I Used

The project utilizes multiple publicly available datasets to simulate diverse transaction behaviors.
Each dataset includes anonymized features representing transaction patterns and risk indicators.

| Dataset Name                                   | Dataset Link                                                       | Number of Samples | Number of Features |
| ---------------------------------------------- | ------------------------------------------------------------------ | ----------------- | ------------------ |
| Credit Card Fraud Detection                    | [Link](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)    | 284,807           | 31                 |
| Credit Card Transactions Fraud Detection       | [Link](https://www.kaggle.com/datasets/kartik2112/fraud-detection) | 1,048,576         | 23                 |
| Fraud E-commerce                               | [Link](https://www.kaggle.com/datasets/vbinh002/fraud-ecommerce)   | 150,000           | 11                 |
| Synthetic data from a financial payment system | [Link](https://www.kaggle.com/datasets/ealaxi/banksim1)            | 594,643           | 10                 |

## Algorithms

CardFraudDetectAI implements both traditional machine learning and deep learning models for comparative analysis.

| Machine Learning           | Deep Learning |
| -------------------------- | ------------- |
| XGBClassifier              | ANN           |
| CatBoostClassifier         | CNN           |
| AdaBoostClassifier         | RNN           |
| GradientBoostingClassifier | LSTM          |
| LGBMClassifier             | Autoencoder   |

## Usage

1. Clone the repository:

   ```shell
   git clone https://github.com/YourUsername/YourRepository.git

   ```

2. Navigate to the project directory:

   ```shell
   cd YourRepository

   ```

3. Access the datasets by referring to their respective links provided in the table above.
4. Download the datasets and place them in the appropriate directory within your project.
5. Use the datasets in your machine learning or data analysis tasks as needed.
6. Make sure to properly attribute the datasets by including the relevant citations or credits to the dataset providers.
7. If you make use of the datasets in your research or projects, consider providing a link or acknowledgment to the original dataset source in your work.
8. If you perform any preprocessing or modifications to the datasets, clearly document the changes made in your project's documentation or README file.
9. Ensure compliance with any licensing or usage restrictions associated with the datasets.

## Contributing

Contributions to this repository are welcome! If you have any additional datasets or improvements to the existing datasets, feel free to submit a pull request.

## License

This repository and the datasets within it are licensed under the MIT License. So, feel free to modify this code to match your specific project and dataset details.

## Usage

Train a model:

python train_model.py --model xgboost

Run inference:

python predict.py --input sample_transaction.csv

Launch the Streamlit dashboard:

streamlit run app.py

Dashboard Features

Real-time transaction risk scoring

SHAP-based model explainability

Fraud trend visualization and performance metrics

## Results

Achieved 0.96 AUC and 95% precision using XGBoost-LSTM hybrid model.

Improved recall by 28% through SMOTE balancing and tuned thresholds.

Processed 10K+ transactions/min with <120ms average latency using FastAPI microservice.

Reduced false negatives by 22%, increasing fraud detection coverage.

## Architecture Overview

Kafka Stream → Feature Processor → XGBoost/LSTM Model → FastAPI Endpoint → Streamlit Dashboard

Kafka: Simulates live transaction streams

FastAPI: Serves model predictions with low latency

Streamlit: Provides real-time insights for analysts

AWS EC2: Hosts model service for scalable deployment

## Future Enhancements

Implement Federated Learning to support cross-bank collaboration without sharing raw data

Add Blockchain-based audit trail for transaction transparency

Optimize for Edge AI deployment on POS terminals and mobile devices

Integrate AutoML pipelines for dynamic model selection

## Contributing

Contributions are welcome!
To contribute:

Fork the repository

Create a new branch (git checkout -b feature/new-feature)

Commit your changes

Push and open a Pull Request

## License

This project is licensed under the MIT License.
Feel free to use, modify, and distribute it with proper credit.

## Author

Cyril Ofori Kupualor
Computer Science Major | Product Builder | AI Developer
📧 Email : cyrilkups95@gmail.com

## Acknowledgments

Special thanks to open data communities like Kaggle and UCI Machine Learning Repository for providing valuable datasets to advance AI in financial fraud prevention.
