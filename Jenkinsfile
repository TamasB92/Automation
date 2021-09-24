pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        sh 'mvn compile'
      }
    }

    stage('Run The test') {
      steps {
        sh 'mvn clean verify'
      }
    }

    stage('sout something') {
      steps {
        sh 'echo "finish"'
      }
    }

  }
}