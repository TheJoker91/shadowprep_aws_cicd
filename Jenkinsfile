pipeline {
    agent any

    environment {
        BRANCH_NAME = 'main'
        GIT_URL = 'https://github.com/TheJoker91/shadowprep_aws_cicd'
    }

    stages {
        stage ('git checkout') {
            steps {
                git branch: "${BRANCH_NAME}", url: "${GIT_URL}"
            }
        }

        stage ('docker build') {
            steps {
                sh 'docker build -t awscicd .'
                sh 'docker images'
            }
        }

        stage ('pwd command') {
            steps {
                sh 'pwd'
            }
        }
    }
}