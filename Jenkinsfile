pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        echo 'Building project'
      }
    }

    stage('Test') {
      steps {
        echo 'Running tests'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying project'
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
