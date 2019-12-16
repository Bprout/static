pipeline  {
    agent any
    stages  {
        stage('Upload to AWS') {
      steps {
          withAWS(region:'us-east-1',credentials:'JenkinsUserCredentials') {
          s3Upload(file:'index.html', bucket:'udabpdevopsc3', path:'')
        }
    }
}
