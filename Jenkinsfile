node {
  stage('init') {
    checkout scm
  }
  stage('build') {
      sh '''
      git pull origin master
      git commit -a -m ""
      git push azure master
      '''
   }  
}
