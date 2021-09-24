pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
  bat "java -version"
  bat "mvn --version"


            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}