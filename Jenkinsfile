pipeline{
    agent any
    environment{
        DIRECTORY_PATH="https://github.com/hirushanirmalt/Deakin-Unit-Page"
        TESTING_ENVIRONMENT="JENKINS"
        PRODUCTION_ENVIRONMENT="Haritha"
    }
    stages{
        stage('Build') {
            steps{
                echo "Building the code using Maven tool"
            }
        }
        stage('Unit and Integration Tests') {
            steps{
                echo "Running unit and integration tests using JUnit tool"
            }
        }
        stage('Code Analysis') {
            steps{
                echo "Conducting code analysis using SonarQube tool"
            }
        }
        stage('Security Scan') {
            steps{
                echo "Running security scans using OWASP ZAP tool"
            }
        }
        stage('Integration tests on Staging') {
            steps{
                echo "Running integration tests  using Phabricator tool"
            }
        }
        stage('Deploy to Production') {
            steps{
                echo "Deploying to production using AWS EC2 instance"
            }
        }
    }
}
