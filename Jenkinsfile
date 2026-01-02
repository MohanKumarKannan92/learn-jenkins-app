pipeline{
    agent any
    stages {
        stage('Without docker') {
            steps {
                echo 'Running without docker!'
            }
        }

        stage('With docker') {
            agent{
                docker{
                    image 'ubuntu:latest'
                }
            }
            steps {
                echo 'Running with docker!'
            }
        }
    }
}