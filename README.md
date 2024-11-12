# Github Actions Tutorial Project

This project demonstrates a simple Flask application. It highlights the integration of **GitHub Actions** for CI/CD with two main steps: testing the application using `pytest` and building/publishing a Docker image. 

## Project Description
The **GithubActionsTutorialProject** provides an end-to-end demonstration of setting up CI/CD pipelines using **GitHub Actions** for a Python Flask app. The project includes automated testing with `pytest` and Dockerization to facilitate continuous deployment. 

### Key Features
- Simple Flask app.
- Automated testing using `pytest`.
- CI/CD pipeline configuration with **GitHub Actions** to automate build, test, and deploy processes.
- Dockerized application for easy deployment.

## Getting Started

### Prerequisites
- Python 3.7 or higher
- Docker
- GitHub account with access to GitHub Actions

### Setup

1. **Clone the repository**:
  ```bash
  git clone https://github.com/username/GithubActionsTutorialProject.git
  cd GithubActionsTutorialProject
  ```
   
2. **Install the required packages**:
  ```bash
  pip install -r requirements.txt
  ```

3. **Run the Flask application**:
  ```bash
  flask run
  ```

4. **Run tests**:
  ```bash
  pytest
  ```

## GitHub Actions Workflow
This project includes a GitHub Actions workflow with two primary jobs:

### 1. Build and Test
  This job performs the following:
 - Checks out the code.
 - Sets up the Python environment.
 - Installs the dependencies from `requirements.txt`.
 - Runs the tests using `pytest` to ensure code functionality.

### 2. Build and Publish
  This job is triggered after a successful test and performs the following:
 - Checks out the code.
 - Sets up Docker Buildx.
 - Logs into DockerHub.
 - Builds and pushes the Docker image to DockerHub.


## Docker Usage
To build and run the Docker container locally:

1. **Build the Docker image**:

  ```bash
  docker build -t flask-app .
  ```

2. **Run the Docker container**:
  ```bash
  docker run -p 5000:5000 flask-app
  ```

## Contributing
 - Fork the project.
 - Create a feature branch (`git checkout -b feature/AmazingFeature`).
 - Commit your changes (`git commit -m 'Add some AmazingFeature`).
 - Push to the branch (`git push origin feature/AmazingFeature`).
 - Open a pull request.


