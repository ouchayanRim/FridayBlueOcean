pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Completed'
      }
    }

    stage('Test1') {
      parallel {
        stage('Test1') {
          steps {
            echo 'Test 1 done'
          }
        }

        stage('Test2 ') {
          steps {
            echo 'Test2 done'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy Completed'
      }
    }

  }
}