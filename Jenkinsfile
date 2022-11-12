pipeline {
    agent any

    stages {
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Sonar Analysis') {
            steps {
                sh 'mvn sonar:sonar \
  -Dsonar.host.url=http://54.89.232.193:9000 \
  -Dsonar.login=4b8bf28f24d8613afebe8093acfd312e86d0b251'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
