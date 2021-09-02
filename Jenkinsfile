pipeline {
  agent any
  stages {
    stage('Log Tool Version') {
      parallel {
        stage('Log Tool Version') {
          steps {
            sh 'python --version'
          }
        }

        stage('check for readme file') {
          steps {
            fileExists 'README.md'
          }
        }

      }
    }

    stage('Print Message') {
      steps {
        echo 'It works!!!'
      }
    }

    stage('Post-Build-Status') {
      steps {
        writeFile(file: 'status.txt', text: 'it really works!!!!')
      }
    }

  }
}