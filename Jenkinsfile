pipeline {
    agent any

    stages {
        stage('Build and Test') {
            parallel {
                stage('Build') {
                    steps {
                        echo 'Building...'
                        sh 'mvn clean install'
                    }
                }
                stage('Test') {
                    steps {
                        echo 'Testing...'
                        sh 'mvn test'
                    }
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add your deployment steps here
            }
        }
    }
}
