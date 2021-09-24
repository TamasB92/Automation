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
  bat "mvn clean install verify"


            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}