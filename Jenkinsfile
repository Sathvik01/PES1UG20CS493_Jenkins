pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ PES1UG20CS493.cpp -o PES1UG20CS493'
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
