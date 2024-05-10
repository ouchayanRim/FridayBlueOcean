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
            input(message: 'yOU W to Build', ok: 'yes sure')
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