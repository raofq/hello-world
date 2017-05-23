pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building..'
      }
    }
    stage('Test') {
      steps {
        parallel(
          "Test": {
            echo 'Testing..'
            
          },
          "test2": {
            echo 'test2...'
            
          }
        )
      }
    }
    stage('Deploy') {
      steps {
        parallel(
          "Deploy": {
            echo 'Deploying....'
            
          },
          "deploy2": {
            echo 'deploy2....'
            
          }
        )
      }
    }
  }
}