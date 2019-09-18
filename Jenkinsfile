pipeline{
    agent 
    node{
     label 'mynode'
     customWorkspace '${JENKINS_HOME}/jobs/${JOB_NAME}/builds/${BUILD_ID}/src/github.com/grugrut/golang-ci-jenkins-pipeline'
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
