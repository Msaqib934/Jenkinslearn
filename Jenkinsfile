pipeline {
    agent any
    environment {
        NEW_VERSION = '1.3.0'
    }
    stages {
        stage('Build') {
            steps {
                echo "Build Maven Project ${NEW_VERSION}"
            }
        }
        stage('Test') {
            when {
                expression {
                    BRANCH_NAME == 'saqib'
                }
            }
            steps {
                echo 'Test Maven Project'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy on Kubernetes'
            }
        }
    }
}
