pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES1UG22CS379 notworking.cpp'
            }
        }
        stage('Test') {
            steps {
                sh './PES1UG22CS379'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
