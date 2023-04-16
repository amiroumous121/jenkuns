pipeline {
    agent any

    environment {
        DIRECTORY_PATH = 'C:\\Users\\john3\\Desktop\\htmlcssforsit223\\Jenkinsfile'
        TESTING_ENVIRONMENT = 'amir121'
        PRODUCTION_ENVIRONMENT = 'amir_jenkins'
    }

    stages {
        stage('Build') {
            steps {
                echo "Fetch the source code from the directory path specified by the environment variable: ${DIRECTORY_PATH}"
                echo "Compile the code and generate any necessary artifacts"
            }
        }

        stage('Test') {
            steps {
                echo "Unit tests"
                echo "Integration tests"
            }
        }

        stage('Code Quality Check') {
            steps {
                echo "Check the quality of the code"
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploy the application to a testing environment specified by the environment variable: ${TESTING_ENVIRONMENT}"
            }
        }

        stage('Approval') {
            steps {
                echo "Waiting for manual approval..."
                sleep(time: 10, unit: 'SECONDS')
                echo "Manual approval received"
            }
        }

        stage('Deploy to Production') {
            steps {
                echo "Deploy the application to the production environment: ${PRODUCTION_ENVIRONMENT}"
            }
        }
    }
}
