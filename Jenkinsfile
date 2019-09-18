pipeline{
    agent 
    node{
     label 'mynode'
     customWorkspace '${JENKINS_HOME}/jobs/${JOB_NAME}/builds/${BUILD_ID}/src/github.com/tazbia-fatima/jenkins_repo'
    }
      tools{
          go 'Go1.13'
      }
    environment{
        G113MODULE = 'on'
    }
    stages{
        stage('Build'){
            steps{
                sh 'go version'
            }
        }
    }
}
