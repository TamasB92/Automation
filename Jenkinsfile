pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        sh '''systeminfo 
cat /etc/os-release
mvn compile'''
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