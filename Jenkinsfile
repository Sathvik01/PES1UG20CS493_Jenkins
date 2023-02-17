pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ PESU.c -o PESU'
                 build job: 'PES1UG20CS493-1', wait: false
                 echo 'Build by CS493 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat PES1UG20CS493.cpp'
                echo 'Test by CS493 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Deploy by CS493 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
