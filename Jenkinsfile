node {
  stage('init') {
    checkout scm
  }
  stage('build') {
      sh '''
      git remote add azure https://junhyun.bae@jenkinstestapp2.scm.azurewebsites.net/JenkinsTestApp2.git
      git push azure master
      '''
   }
  
}
