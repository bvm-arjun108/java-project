pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Starting build...'
                sh 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                echo 'Starting tests...'
                sh 'mvn test'
            }
        }
    }
}
