pipeline {
  agent any

  environment {
    APP_VERSION = "1.3.0"
  }

  stages {
    stage('Build') {
      steps {
        echo 'Building project'
        echo "Building version ${APP_VERSION}"
      }
    }

    stage('Test') {
      steps {
        echo 'Testing project'
        echo "Testing version ${APP_VERSION}"
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying project'
        echo "Deploying version ${APP_VERSION}"
      }
    }
  }

  post {
    always {
      echo 'Post build condition running'
    }
    success {
      echo 'Build completed successfully'
    }
    failure {
      echo 'Post action: Build failed'
    }
  }
}
