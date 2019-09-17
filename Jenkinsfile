node {
    // Install the desired Go version
    def root = tool name: 'Go 1.8', type: 'go'
 
    // Export environment variables pointing to the directory where Go was installed
    withEnv(["GOROOT=${root}", "PATH+GO=${root}/bin"]) {
        sh 'go version'
    }
    }
pipeline{
   agent any
    stages{
        stage('Build-go'){
            steps{
                sh 'echo Building'
                sh 'go build hello.go'
            }
        }
        stage('Test'){
            steps{
               echo "what to do next?"
            }
        }
    }
}
            
