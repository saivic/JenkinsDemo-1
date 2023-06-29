pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from the repository
                git 'https://github.com/saivic/JenkinsDemo-1.git'
            }
        }

        stage('Build') {
            steps {
                // Build the Spring Boot application using Maven
                bat 'mvn clean install'
            }
        }

        
        stage('Deploy') {
            steps {
            	bat 'start java -jar C:/Users/Administrator/Documents/workspace-spring-tool-suite-4-4.19.0.RELEASE/JenkinsDemo/target/JenkinsDemo-0.0.1-SNAPSHOT.jar'
            }
        }
    }
}
