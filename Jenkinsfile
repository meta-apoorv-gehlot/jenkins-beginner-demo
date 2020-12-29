pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('run') {
            steps {
                sh 'java -jar target/gs-maven-0.1.0.jar'
            }
        }
    }
}