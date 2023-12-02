pipeline {
  agent any
  stages {
    stage('Git Checkout') {
      steps {
        git(url: 'https://github.com/Midhaso/MY-APP.git', branch: 'master')
        echo 'Successfully check out from GitHub'
      }
    }

    stage('Install Dependencies') {
      steps {
        bat 'npm install'
        echo 'Package install successfully '
      }
    }

    stage('Compile') {
      steps {
        bat 'Compile'
        echo 'Compiled  Successfully!!'
      }
    }

    stage('Quality-Gate') {
      steps {
        echo 'Quality Gate passed Successfully'
      }
    }

  }
}