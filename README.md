

# CI/CD Pipeline with Jenkins, Maven, SonarQube, Trivy, and Kubernetes

This project demonstrates the creation of a Continuous Integration and Continuous Deployment (CI/CD) pipeline using various tools like Jenkins, Maven, SonarQube, Trivy, Docker, Nexus Repository, and Kubernetes. The project follows best practices for software development and deployment, ensuring code quality, security, and smooth integration of services.

> **Note:** This project was created by referencing the [Aditya Jaiswal YouTube video](https://www.linkedin.com/in/adityajaiswal7/).


## Table of Contents

- [Project Overview](#project-overview)
- [Tools Used](#tools-used)
- [Pipeline Workflow](#pipeline-workflow)
- [Installation and Setup](#installation-and-setup)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

# Project Overview

This project is a demonstration of a robust CI/CD pipeline that integrates multiple tools to ensure high code quality and secure deployments. The pipeline includes the following steps:

1. **Code Versioning**: The source code is hosted on GitHub.
2. **Continuous Integration**: Jenkins automates the build, testing, and code analysis processes.
3. **Code Quality Analysis**: SonarQube is used to ensure code quality by analyzing code for bugs, vulnerabilities, and code smells.
4. **Security Scanning**: Trivy is used to scan the application and Docker images for vulnerabilities.
5. **Artifact Management**: Maven builds the project and stores the artifacts in Nexus Repository.
6. **Continuous Deployment**: The application is deployed to Kubernetes, where it is continuously monitored and updated.

## Tools Used

- **GitHub**: For version control and source code management.
- **Jira**: For project management and tracking.
- **Jenkins**: For automating the CI/CD pipeline.
- **Maven**: For project build management.
- **SonarQube**: For static code analysis and code quality checks.
- **Trivy**: For security vulnerability scanning.
- **Nexus Repository**: For artifact storage and management.
- **Docker**: For containerization of the application.
- **Kubernetes**: For container orchestration and deployment.

## Pipeline Workflow

The pipeline workflow is as follows:

1. **Developer Pushes Code to GitHub**
   - Code is pushed to the GitHub repository.
   - Jenkins is triggered to start the pipeline.

2. **Code Checkout and Build**
   - Jenkins checks out the code from GitHub.
   - Maven is used to compile the code and run unit tests.

3. **Code Quality Analysis**
   - SonarQube analyzes the code for quality metrics.
   - If the code passes the quality gate, it proceeds to the next step.

4. **Security Scanning**
   - Trivy scans the code and Docker images for vulnerabilities.
   - Any critical issues found are reported and must be fixed before proceeding.

5. **Build and Publish Artifact**
   - Maven builds the project and stores the artifacts in the Nexus Repository.
   - Docker images are built and pushed to Docker Hub.

6. **Deployment to Kubernetes**
   - The application is deployed to the Kubernetes cluster.
   - Deployment is verified, and notifications are sent.

7. **Monitoring and Security**
   - The application is continuously monitored in the Kubernetes environment.
   - Trivy scans the running containers for vulnerabilities.

## Installation and Setup

To set up this project, follow these steps:

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/your-repository.git
   cd your-repository
   ```

2. **Install Required Tools**
   - [Install Jenkins, Maven, Docker, SonarQube, Trivy, Nexus, and Kubernetes.](https://github.com/Adityalodhi/CICD-PIPELINE/tree/main/CIDI%20pipeline%20Codes/PHASE-1)

3. **Configure Jenkins**
   - [Set up Jenkins with required plugins and configure the pipeline script.](https://github.com/Adityalodhi/CICD-PIPELINE/blob/main/CIDI%20pipeline%20Codes/PHASE-1/Jenkins.md)

4. **Set Up SonarQube**
   - [Install and configure SonarQube for static code analysis.](https://github.com/Adityalodhi/CICD-PIPELINE/blob/main/CIDI%20pipeline%20Codes/PHASE-1/Sonarqube.md)

5. **Configure Trivy**
   - [Set up Trivy for scanning Docker images.](https://github.com/Adityalodhi/CICD-PIPELINE/blob/main/CIDI%20pipeline%20Codes/PHASE-1/trivet.md)

6. **Deploy to Kubernetes**
   - [Configure Kubernetes and deploy the application.](https://github.com/Adityalodhi/CICD-PIPELINE/blob/main/CIDI%20pipeline%20Codes/PHASE-1/2.%20K8-Setup.md)

## Usage

To run the pipeline:

1. Push code to the GitHub repository.
2. Jenkins will automatically trigger the pipeline.
3. Monitor the pipeline progress via Jenkins.
4. Review the SonarQube and Trivy reports.
5. Once the pipeline completes, the application will be deployed to Kubernetes.

## Images

![jenkins](https://github.com/user-attachments/assets/6359d113-1892-4fd7-b99a-2d1ffa96d334)
![node exp grapgana](https://github.com/user-attachments/assets/4b5b29ee-ba95-4115-800d-e2288fde45c4)
![prometheus black box monitoring](https://github.com/user-attachments/assets/065be8e5-d201-43c4-a278-e19d087106bb)
![nexus](https://github.com/user-attachments/assets/d7c38702-0dd4-4415-9ffb-113ff3f59e1c)
![sonarqube](https://github.com/user-attachments/assets/254e6dad-e362-438a-8a05-649bafa0ad4c)
![docker hub](https://github.com/user-attachments/assets/5ef7d803-77b7-4600-9781-f21fa1df5444)
![servers](https://github.com/user-attachments/assets/d72d3c4c-9541-4e03-844d-0f9937f6e0ee)
