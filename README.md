# Nyenyak Cloud Computing Documentation
## Project Summary
Nyenyak uses Google Cloud Platform (GCP) and Firebase to develop a system capable of classifying sleep disorders, such as insomnia and sleep apnea, based on user data. Additionally, the system will provide actionable suggestions to enhance the sleep quality of users experiencing sleep disturbances. The project involves a collaboration between machine learning, mobile development, and cloud computing teams

## Cloud Architecture
![Architecture Illustration](https://github.com/canggihwr/cc-doc/blob/main/infrastructure.jpg)

## 1. Setup Google Cloud Platform

- Create Project & Configure Identity and Access Management.
- Enable the following APIs:
  - App Engine API
  - Cloud Run Admin API
  - Google Container Registry API
  - Firebase API (Management, Realtime Database, etc.)
  - Cloud Monitoring API
  - Cloud Logging API

## 2. Setup Firebase

- Open [Firebase](https://firebase.google.com/), go to the console, and connect it to your Google Cloud Project.
- Activate Firebase Auth & Firebase Realtime Database.
- Create a **Service Account** and download the `seviceAccountKey.json` file .

## 3. Clone Project and Set Google Cloud Account

- Open your preferred code editor (Visual Studio Code).
- Clone the Nyenyak project from [Nyenyak-Backend-Repo](https://github.com/w0n0g1ren/Nyenyak/tree/BackEnd) using the command `git clone -b BackEnd https://github.com/w0n0g1ren/Nyenyak.git`.
- Initialize a Git repository with `git init` and connect it to your Google Cloud account.

## 4. Set Project and Deploy Application

- In the terminal, set your project by executing `gcloud config set project nyenyak-project-dev`.
- Deploy both nodeJS and model API to App Engine and Cloud Run.

## 6. API Documentation

- For API Documentation, refer to the following link: [API Documentation](https://docs.google.com/document/d/1qCDyOA_lNiGtEkrO0boCFtzEbLcFK6LTec5WuPWMv50/edit?usp=sharing)
![API Image](insert_link_to_your_api_image)

**Additional Backend Details:**
- Backend API is built using Node Express.js to handle user authentication, diagnosis, articles, and user details.
- We deployed the backend API to App Engine for easier scalability and reliability.
- A separate the API for TensorFlow model, built using Flask and deployed to Cloud Run.
- Utilize Cloud Monitoring & Logging for comprehensive resource monitoring and alerting.

## Conclusion

The Nyenyak project integrates Google Cloud Platform and Firebase Realtime Database to create a robust and scalable solution. The backend architecture ensures efficient communication between the mobile app, backend API, and machine learning model, providing users with accurate sleep disorder diagnoses and solution for improvement.


===============================================

# Nyenyak: A Cloud-Based System for Sleep Disorder Diagnosis and Improvement

![Nyenyak Logo](insert_link_to_your_logo_image)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Status: Active](https://img.shields.io/badge/Status-Active-green.svg)](https://github.com/your_username/Nyenyak-Backend-Repo)
[![Version: 1.0.0](https://img.shields.io/badge/Version-1.0.0-blue.svg)](https://github.com/your_username/Nyenyak-Backend-Repo/releases/tag/v1.0.0)
[![Contributors: 5](https://img.shields.io/badge/Contributors-5-orange.svg)](https://github.com/your_username/Nyenyak-Backend-Repo/graphs/contributors)

Nyenyak is a cloud-based system that uses machine learning to diagnose sleep disorders and provide personalized suggestions for improvement. It leverages Google Cloud Platform and Firebase services to create a scalable and reliable solution that connects users, mobile apps, backend APIs, and machine learning models.

## Table of Contents

- [Nyenyak: A Cloud-Based System for Sleep Disorder Diagnosis and Improvement](#nyenyak-a-cloud-based-system-for-sleep-disorder-diagnosis-and-improvement)
  - [Table of Contents](#table-of-contents)
  - [Cloud Architecture](#cloud-architecture)
  - [Setup Google Cloud Platform](#setup-google-cloud-platform)
  - [Download Google Cloud SDK and Run Cloud Shell in Your Code Editor](#download-google-cloud-sdk-and-run-cloud-shell-in-your-code-editor)
  - [Setup Firebase](#setup-firebase)
  - [Clone Project and Set Google Cloud Account](#clone-project-and-set-google-cloud-account)
  - [Set Project and Deploy Application to App Engine](#set-project-and-deploy-application-to-app-engine)
  - [REST-API](#rest-api)
  - [Testing](#testing)
  - [Contributing](#contributing)
  - [Issues and Features](#issues-and-features)
  - [License](#license)

## Cloud Architecture

![Architecture Illustration](https://github.com/canggihwr/cc-doc/blob/main/infrastructure.jpg)

## Setup Google Cloud Platform

- Create Project & Configure Identity and Access Management.
- Enable the following APIs:
  - App Engine API
  - Cloud Run Admin API
  - Compute Engine API
  - Cloud Logging API
  - Firebase Realtime Database API
  - Cloud Pub/Sub API
  - Cloud Build API
  - Cloud Scheduler API

## Download Google Cloud SDK and Run Cloud Shell in Your Code Editor

- Ensure you have Git, a code editor (Visual Studio Code), and a Google Cloud Account installed.

## Setup Firebase

- Open [Firebase](https://firebase.google.com/), go to the console, and connect it to your Google Cloud Project.
- Activate Firebase Auth & Firebase Realtime Database.
- Create a **Service Account** and download the corresponding file.

## Clone Project and Set Google Cloud Account

- Open your preferred code editor (Visual Studio Code).
- Clone the Nyenyak project from [Nyenyak-Backend-Repo](insert_link_to_your_backend_repo) using the command `git clone https://github.com/your_username/Nyenyak-Backend-Repo.git`.
- Initialize a Git repository with `git init` and connect it to your Google Cloud account.

## Set Project and Deploy Application to App Engine

- In the terminal, set your project by executing `gcloud config set project your-project`.
- Add any additional deployment instructions specific to your project.

## REST-API

- For API Documentation, refer to the following link: [API Documentation](insert_link_to_your_api_documentation)
![API Image](insert_link_to_your_api_image)

**Additional Backend Details:**
- Backend API is built using Node.js and Express.js to handle user authentication, diagnosis, articles, and user details.
- Deployed backend API to App Engine for scalability and reliability.
- A separate API for TensorFlow model, built by the ML team using Flask, is deployed to Cloud Run.
- Utilize Cloud Monitoring & Logging for comprehensive resource monitoring and alerting.

## Testing

- To test the project, run the command `npm test` in the terminal.
- The project uses [Mocha](https://mochajs.org/) and [Chai](https://www.chaijs.com/) as the testing frameworks and tools.
- The code coverage report is generated by [Istanbul](https://istanbul.js.org/).
- The code coverage badge is created by [Codecov](https://codecov.io/).

[![codecov](https://codecov.io/gh/your_username/Nyenyak-Backend-Repo/branch/master/graph/badge.svg?token=YOUR_TOKEN)](https://codecov.io/gh/your_username/Nyenyak-Backend-Repo)

## Contributing

- We welcome contributions from anyone who is interested in improving the project.
- To contribute, please follow these steps:
  - Fork the repository and create your branch from `master`.
  - Clone the forked repository and install the dependencies with `npm install`.
  - Make your changes and commit them with a descriptive message.
  - Push your changes to your branch and create a pull request to the `master` branch of the original repository.
  - Wait for your pull request to be reviewed and merged.
- Please adhere to the [Code of Conduct](insert_link_to_your_code_of_conduct) and respect the other contributors.
- You can also check the [Contributors](insert_link_to_your_contributors) page to see who has contributed to the project.

## Issues and Features

- If you encounter any issues or bugs while using the project, please report them to the [Issue Tracker](insert_link_to_your_issue_tracker).
- If you have any ideas or suggestions for new features or enhancements, please create a [Feature Request](insert_link_to_your_feature_request).
- Please use the [Issue Template](insert_link_to_your_issue_template) and the [Feature Request Template](insert_link_to_your_feature_request_template) to create your issues and feature requests.

## License

- The project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
- This means that you can use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the project, as long as you give appropriate credit and include the license notice in any copies.
- You can find the full license text [here](insert_link_to_your_license_text).
