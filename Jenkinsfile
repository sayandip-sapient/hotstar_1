pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Checkout the source code from version control
                checkout scm

                // Build the Spring Boot application with Maven
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                // Run tests
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                // Deploy the Spring Boot application (replace with your deployment command)
                // sh 'java -jar target/your-spring-boot-app.jar'
            }
        }
    }
}
