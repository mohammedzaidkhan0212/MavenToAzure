pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'mvn clean install'
            }
        }
        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }
        stage('Run Application') {
            steps {
                bat 'java -jar target/Azure-0.0.1-SNAPSHOT.jar'
            }
        }
    }
}
