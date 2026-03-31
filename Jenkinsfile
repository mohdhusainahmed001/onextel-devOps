pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/<mohdhusainahmed001>/<onextel-devOps>.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'   // Replace with your build tool
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'            // Replace with your test command
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
}
