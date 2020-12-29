pipeline {
    agent any
    tools { 
        maven 'Maven 3.3.9' 
        jdk 'jdk8' 
    }
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