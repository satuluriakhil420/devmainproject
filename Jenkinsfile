pipeline {
    agent any

    stages {
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn build'
            }
        }
        stage('Deploy') {
            steps {
                echo 'print deploy....'
            }
        }
    }
}
