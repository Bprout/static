pipeline {
     agent any
     stages {
       stage('UploadAWS') {
         steps {
            withAWS(region:'us-east-1',credentials:'JenkinsUserCredentials') {
              s3Upload(bucket: 'udabpdevopsc3', file:'index.html', includePathPattern:'**/*');
            }
       }
     }
}
  
