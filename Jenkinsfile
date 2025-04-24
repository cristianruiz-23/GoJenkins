pipeline {
     agent { label 'agent4' }


    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/cristianruiz-23/GoJenkins.git'
            }
        }
        stage('Build') {
            steps {
                sh 'go build ./...'
            }
        }
        stage('Test') {
            steps {
                sh 'go test ./...'
            }
        }
    }
}