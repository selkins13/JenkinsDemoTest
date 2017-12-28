pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                go build HelloWorld.go
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                ./HelloWorld
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
