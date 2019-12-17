pipeline {
    agent any
    stages {
      stage(Lint HTML) {
        steps {
          sh 'tidy -q -e *.html'
        }
      }
      stage('UploadAWS') {
        steps {
          withAWS(region:'us-east-1',credentials:'JenkinsUserCredentials') {
          s3Upload(file:"index.html",bucket:'udabpdevopsc3',path:'*/*')
          }
        }
      }
    }
}
