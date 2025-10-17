pipeline {
    agent any
    stages{
        stage('Build Frontend') {
            steps {
                sh 'python3 app.py' 
                }
        }
    }
  // Post Actions
  post {
      success {
          echo 'Deployment Successful!'
      }
      failure {
          echo 'Deployment Failed! Check Console Output for errors.'
      }
  }
}
