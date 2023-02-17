pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES1UG20CS117 PES1UG20CS117-1.cpp'
                echo 'Successfully Compiled PES1UG20CS117-1.cpp file'
            }
        }
        stage('Test') {
            steps {
                sh './PES1UG20CS117'
                echo 'Successfully Printed Output of PES1UG20CS117-1.cpp file'

        }
        }
        stage('Deploy') {
            steps {
                echo 'PES1UG20CS117 Deployment Successful'
            
        }
    }
    }
    post {
        failure {
            error "PES1UG20CS117 Pipeline Failed"
            }
        }
    }
