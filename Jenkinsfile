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
         sh   'java -version'
          }
        }

        stage('ceva') {
          steps {
            sh 'java'
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