pipeline {
  
    agent any
  environment {
        NEW_VERSION = '1.1.1'  
  }
  stages {
    
    stage("build") {
      steps {
            echo 'Building the application ...'
            echo "Version ${NEW_VERSION}"
            }
      }
    
    stage("test") {   
      steps {
          echo 'Testing the application ...'
          }
      }
    
    stage("deploy") {
      steps {
            echo 'Deploying the application ...'
            }
       }
  }
  post {
    always {
           echo 'Build completed ...'
    }
    success {
            echo 'Build successful ...'
    }
    failure {
            echo 'Build failed ...'
    }
  }
}
