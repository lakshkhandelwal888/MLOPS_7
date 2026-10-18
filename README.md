# MLOps CI/CD Pipeline Using GitHub Actions

## Aim
To implement a CI/CD pipeline for a machine learning project using GitHub Actions to automate code validation, testing, and deployment.

## Project Overview
This project uses the Iris dataset to train a Logistic Regression classifier. The model is evaluated using accuracy and a classification report. Pytest is used to validate model accuracy automatically.

## Project Structure
```text
CICD_7/
├── .github/
│   └── workflows/
│       └── cicd.yml
├── src/
│   └── model.py
├── tests/
│   └── test_model.py
├── requirements.txt
├── app.py
└── README.md
```

## Technologies Used
- Python
- Scikit-learn
- Pytest
- GitHub Actions

## Execution
Run the model:
```bash
python src/model.py
```

Run the application:
```bash
python app.py
```

Run automated tests:
```bash
pytest -v
```

## CI/CD Workflow
The GitHub Actions workflow runs when code is pushed to the main branch or a pull request is created for main. It installs dependencies, executes unit tests, and runs a deployment simulation after successful tests.

## Expected Outcome
The workflow automatically tests the machine learning application and permits the deployment simulation only when the tests pass.