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

        stage('test3') {
          steps {
            input(message: 'are you to deploy', ok: 'Yes I am sure')
            echo 'Test 3 tested'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy Completed'
      }
    }

    stage('Notify for new Build') {
      steps {
        echo 'Nex Buld Completed'
      }
    }

  }
}