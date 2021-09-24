pipeline {
  agent any
  stages {
    stage('check for pom') {
      steps {
        fileExists 'pom.xml'
      }
    }

    stage('Build with maven') {
      parallel {
        stage('Build with maven') {
          steps {
            sh '''java -version;
sdk use java  8.0.302-zulu;
mvn compile clean verify'''
          }
        }

        stage('ceva') {
          steps {
            powershell 'java -version'
          }
        }

      }
    }

    stage('Post build') {
      steps {
        writeFile(file: 'status.txt', text: 'hey it works')
      }
    }

  }
}