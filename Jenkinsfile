pipeline {
    agent any

    stages {
        stage ('Pre-Test') {
            steps {
                echo 'Pre-test..'
                sh 'go run hello.go'
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'go build hello.go'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh './hello'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
