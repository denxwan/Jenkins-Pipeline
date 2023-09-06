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
                echo "Fetch the source code from the directory path ($DIRECTORY_PATH) specified by the environment variable"
                echo "Compile the code and generate anby necessary artifacts"
            }
        }
        stage('Test') {
            steps{
                echo "=====UNIT-TESTS====="
                echo "=====INTEGRATION-TESTS====="
            }
        }
        stage('Code Quality Check') {
            steps{
                echo "Check the quality of the code"
            }
        }
        stage('Deploy') {
            steps{
                echo "Deploy the application to a testing environment ($TESTING_ENVIRONMENT) specified by the environment variable"
            }
        }
        stage('Approval') {
            steps{
                sleep 10
            }
        }
        stage('Deploy to Production') {
            steps{
                echo "Deployed to the $PRODUCTION_ENVIRONMENT production environment"
            }
        }
        stage('Complete') {
            steps{
                echo "Completed"
            }
        }
    }
}
