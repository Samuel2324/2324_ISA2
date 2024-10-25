pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                script {
                    bat "docker build -t 2324 ."
                }
            }
        }


        stage('Delete container named 2324') {
            steps {
                script {
                    bat "docker rm --force 2324"
                }
            }
        }

        stage('Run Docker Container') {
            steps {
                script {
                    bat "docker run -d --name 2324 2324"
                }
            }
        }
    }
}
