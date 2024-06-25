pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build Maven Project'
            }
        }
        stage('Test') {
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
