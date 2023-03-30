pipeline {
    agent any
    
    stages {
        stage('Build') {
            environment {
                // specify the Maven installation to use
                MVN_HOME = tool 'Maven 3.8.7'
                PATH = "${MVN_HOME}/bin:${PATH}"
            }
            steps {
                echo 'Starting build...'
                sh 'mvn clean install'
            }
        }
        stage('Test') {
            environment {
                // specify the Maven installation to use
                MVN_HOME = tool 'Maven 3.8.7'
                PATH = "${MVN_HOME}/bin:${PATH}"
            }
            steps {
                echo 'Starting tests...'
                sh 'mvn test'
            }
        }
    }
}
