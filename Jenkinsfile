pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                bat 'mvn clean package'
            }
        }
        stage('run') {
            steps {
                bat 'java -jar target/gs-maven-0.1.0.jar'
            }
        }
    }
}