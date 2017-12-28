pipeline {
    agent any

    node {
      checkout scm

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                python hello.py
                  }
              }
            }
        }
      }
