pipeline {
    agent any

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
