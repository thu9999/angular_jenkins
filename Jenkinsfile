pipeline{
    agent any
    stages{
        stage("w/o docker"){
            steps{
                sh 'echo "Without docker"'
            }
        },
        stage('w/ docker'){
            agent {
                image: node:18-alpine
            }
            steps {
                sh 'echo "With docker"'
            }
        }
    }
}