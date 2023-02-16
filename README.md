Customer Churn Prediction

This project is a machine learning solution to predict customer churn using transactional data. It uses XGBoost classifier to predict whether a customer is likely to churn or not.

Usage

To use this project, you will need Docker installed on your machine. You can download Docker from the official website.

Once you have Docker installed, clone this repository and navigate to the project directory:

```bash
git clone https://github.com/your-username/your-repository.git
cd your-repository
```

Build the Docker image using the following command:

```bash
docker build -t customer-churn .
```
This command will build a Docker image with the name customer-churn.

To run the Docker container and generate predictions, use the following command:

```
docker run customer-churn
```
