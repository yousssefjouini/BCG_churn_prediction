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
docker run -v /path/to/input/data:/app/data -v /path/to/output:/app/output customer-churn
```
This command will start a Docker container with the name customer-churn, mount the input data directory to the /app/data directory inside the container, and mount the output directory to the /app/output directory inside the container.
docker run -v /path/to/input/data:/app/data -v /path/to/output:/app/output customer-churn

You can modify the input data by updating the file at /path/to/input/data/transactions.csv. The output of the container will be a file at /path/to/output/predictions.csv containing the predicted churn probabilities for each customer.

Development

To run the tests, use the following command:

```bash
Copy code
docker run -v /path/to/repo:/app -w /app customer-churn poetry run pytest
```

This command will start a Docker container with the name customer-churn, mount the repository directory to the /app directory inside the container, set the working directory to /app, and run the tests using Poetry.

The project follows PEP 8 coding style and is formatted using Black. To format the code, use the following command:

```bash
docker run -v /path/to/repo:/app -w /app customer-churn poetry run black .
```
This command will start a Docker container with the name customer-churn, mount the repository directory to the /app directory inside the container, set the working directory to /app, and format the code using Black.
