pipeline {
    agent {
        // specify the Maven installation to use
        tools {
            maven 'Maven 3.8.7'
        }
    }
    
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

