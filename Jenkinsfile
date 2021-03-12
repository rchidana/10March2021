pipeline {
  agent any
  stages {
    stage('Git Checkout') {
      steps {
        git(url: 'https://github.com/rchidana/Accenture_Pipeline.git', branch: 'master')
        echo 'Checkout Code'
        bat 'Compile.bat'
      }
    }

    stage('Deploy') {
      steps {
        bat 'Deploy.bat'
      }
    }

  }
}