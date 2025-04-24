pipeline {
    agent { label 'agent4' }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/cristianruiz-23/GoJenkins.git'
            }
        }
        stage('Test') {
            steps {
                sh 'go test ./... -v -json > result.json'
            }
        }
    }


}