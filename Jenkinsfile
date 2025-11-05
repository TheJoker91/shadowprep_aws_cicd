pipeline {
    agent any

    stages {
        stage ('git checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/TheJoker91/shadowprep_aws_cicd'
            }
        }

        stage ('test') {
            steps {
                sh 'echo test'
            }
        }

        stage ('pwd command') {
            steps {
                sh 'pwd'
            }
        }
    }
}