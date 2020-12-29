pipeline {
    // agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            withMaven {
                sh 'mvn clean package'
            }
        }
        stage('run') {
            withMaven {
                sh 'java -jar target/gs-maven-0.1.0.jar'
            }
        }
    }
}