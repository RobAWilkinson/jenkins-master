pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
				checkout scm
      }
    }
    stage("Echo") {
      steps {
        echo "test"
        sh "ls nest"
        sh "ls nest/double-nested"
      }
    }
  }
}
