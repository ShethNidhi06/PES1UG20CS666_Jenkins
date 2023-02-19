pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o nidhi_task5 nidhi_task5.cpp'
                build job: 'PES1UG20CS666-1'
                echo 'build stage successful'
            }
        }
        stage('Test') {
            steps {
                sh './nidhi_666'
                echo 'test stage successful'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying "'
                echo 'deployment successful'
            }
        }
    }
    post {
        failure {
          echo 'pipeline failed'
                }
            
        
    }
}
