pipeline {
    // Run on an agent where we want to use Go
    node {
      // Install the desired Go version
      def root = tool name: 'Go 1.8', type: 'go'

      // Export environment variables pointing to the directory where Go was installed
      withEnv(["GOROOT=${root}", "PATH+GO=${root}/bin"]) {
      sh 'go version'
        }
      }

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
