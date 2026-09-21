# CI/CD Task 1

A simple Python project demonstrating a basic CI pipeline using GitHub Actions.

## Project Features

- Python application
- Unit testing with **pytest**
- Code linting with **Ruff**
- Docker image build
- Automated CI checks with **GitHub Actions**
- CI runs on pushes and pull requests

## Project Structure

- [CI Workflow](https://github.com/Haashim1/CI-Workflow) — GitHub Actions workflow for automated CI checks
- [.gitignore](https://github.com/Haashim1/CI-Workflow/blob/main/.gitignore) — Specifies files and folders that Git should ignore
- [Dockerfile](https://github.com/Haashim1/CI-Workflow/blob/main/Dockerfile) — Defines the Docker image build configuration
- [app.py](https://github.com/Haashim1/CI-Workflow/blob/main/app.py) — Contains the Python application
- [requirements.txt](https://github.com/Haashim1/CI-Workflow/blob/main/requirements.txt) — Lists the Python dependencies
- [test_app.py](https://github.com/Haashim1/CI-Workflow/blob/main/test_app.py) — Contains the unit tests

## How the CI Pipeline Works

Whenever code is pushed to GitHub or a pull request is created, GitHub Actions automatically:

1. Checks out the repository
2. Sets up Python
3. Installs the dependencies
4. Runs Ruff for code linting
5. Runs unit tests with pytest
6. Builds the Docker image

If all steps pass, the CI workflow is marked as successful.

## Running Locally

### Install Dependencies

```bash
python -m pip install -r requirements.txt
```

### Run Unit Tests

```bash
python -m pytest
```

### Run Linting

```bash
python -m ruff check .
```

### Build the Docker Image

```bash
docker build -t cicd-task1 .
```

### Run the Docker Container

```bash
docker run --rm cicd-task1
```

## Technologies Used

- Python
- Pytest
- Ruff
- Docker
- Git
- GitHub Actions

## Result

The CI/CD pipeline was successfully implemented and tested.

GitHub Actions successfully completed:

- Code linting with Ruff
- Unit tests with pytest
- Docker image build

All configured CI checks passed successfully, confirming that the project is working as expected.

<img width="1405" height="659" alt="CI" src="https://github.com/user-attachments/assets/724c9ca6-4c42-4163-a97c-adb03a2f1a40" />
