pipeline {
  agent any
  triggers { cron('*/5 * * * *') }
  stages {
    stage('Build') {
      steps {
        echo "now building from build number ${BUILD_NUMBER}"
        echo 'whats really good??'
      }
    }
    stage('Test'){
      steps {
        echo "now testing from build number ${BUILD_NUMBER}"
        echo 'whats really good??'
      }
    }
    stage('Deploy'){
      steps {
        echo "now deploying from build number ${BUILD_NUMBER}"
        echo 'the build duration is ${currentBuild.duration}'
      }
    }
  }
  post { always { echo 'I will always be here Jenkins. ' } }
}
