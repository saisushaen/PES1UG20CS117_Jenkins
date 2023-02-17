pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ -o PES1UG20CS117 PES1UG20CS117-1.cpp'
      }
    }
    stage('Test') {
      steps {
        sh './PES1UG20CS117'
      }
    }
    stage('Deploy') {
      steps {
        echo 'PES1UG20CS117 deployed successfully'
      }
    }
  }
  
  post {
    failure{
      error "PES1UG20CS117 Pipeline Failed"
    }
  }
}
