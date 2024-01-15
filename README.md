* * *

Geto-Server
===========

Welcome to the Geto-Server repository! This repository contains a Quarkus-based Java application designed for deployment to Azure Web App Service, with an automated CI/CD pipeline using GitHub Actions.

Overview
--------

This project demonstrates a streamlined process for building and deploying a Java application. It leverages GitHub Actions for continuous integration and deployment (CI/CD) and Azure Web App Service for hosting the application.

Getting Started
---------------

### Prerequisites

*   Java Development Kit (JDK)
*   Maven (for building the Java application)
*   Git (for version control)
*   Access to Azure cloud services
*   A GitHub account

### Setting Up for Local Development

1.  **Clone the Repository**:
    
    bashCopy code
    
    `git clone https://github.com/scanalesespinoza/geto-server.git cd geto-server`
    
2.  **Local Build**: Use Maven to build the application:
    
    bashCopy code
    
    `mvn clean package`
    
3.  **Run Locally**: After a successful build, run the application locally to test:
    
    bashCopy code
    
    `java -jar target/geto-server-1.0.0-SNAPSHOT-runner.jar`
    

### Continuous Integration and Deployment

The repository is configured with GitHub Actions for CI/CD, automating the process of building, testing, and deploying the application to Azure Web App Service.

#### GitHub Actions Workflow

*   The workflow is defined in the `.github/workflows` directory.
*   It triggers on pushes to the main branch, handling build and deployment.

#### Azure Configuration

*   The application is set up to deploy to Azure Web App Service.
*   Necessary configurations, including environment variables and service principal credentials, are securely stored in GitHub Secrets.

### Automated Environment Management

*   The project includes automation for managing the Azure Web

App Service, specifically for scheduling start and stop times using Azure Automation or Logic Apps.

*   This setup helps in optimizing costs, especially for non-production environments.

Contribution
------------

Contributions to the Geto-Server project are welcome! If you have suggestions or improvements, feel free to fork the repository and submit a pull request.

Issues
------

If you encounter any issues or have questions, please file them in the repository's Issues section.

License
-------

This project is licensed under the [MIT License](LICENSE.md) - see the LICENSE file for details.

* * *
