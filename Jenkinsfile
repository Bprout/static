pipeline {
     agent any
     stages {
       stage('Build') {
         steps {
            withAWS(region:'us-east-1',credentials:'JenkinsUserCredentials') {
              s3Upload(bucket: 'udabpdevopsc3', file:'index.html', includePathPattern:'**/*');
            }
       }
     }
}
  
