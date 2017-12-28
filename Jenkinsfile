pipeline {
    agent any

    stages {
        node {
            checkout scm

            stage('Build') {
            steps {
                echo 'Building..'
                python hello.py
              }
            }
        }
    }
}
