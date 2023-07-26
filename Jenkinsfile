pipeline {
  agent any
  stages {
    stage('checkoutGit') {
      steps {
        git(url: 'https://github.com/Rahmon22SoH/BlueOceanDamo.git', branch: 'main')
      }
    }

    stage('build') {
      steps {
        echo 'this ra'
      }
    }

    stage('deploy dev1') {
      parallel {
        stage('deploy dev1') {
          steps {
            echo 'dev1'
            sleep 10
          }
        }

        stage('deploy dev2') {
          steps {
            echo 'microsev 2'
            sleep 15
          }
        }

      }
    }

    stage('test') {
      steps {
        echo 'testing /////'
      }
    }

  }
}