pipeline {
  agent any
  stages {
    stage('Log tool version') {
      parallel {
        stage('Log tool version') {
          steps {
            sh '''mvn --version
'''
          }
        }

        stage('check for pom') {
          steps {
            fileExists 'pom.xml'
          }
        }

      }
    }

    stage('Build with maven') {
      steps {
        sh 'mvn compile clean verify'
      }
    }

    stage('Post build') {
      steps {
        writeFile(file: 'status.txt', text: 'hey it works')
      }
    }

  }
}