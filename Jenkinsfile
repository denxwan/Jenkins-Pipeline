pipeline{
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
            post{
                success{
                    mail to: "harithadenuwan01@gmail.com",
                    subject: "Tests status Email",
                    body: "Tests were successful"
                }
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
            post{
                success{
                    mail to: "harithadenuwan01@gmail.com",
                    subject: "Security scan status Email",
                    body: "Security scan was successful"
                }
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
