node {
  stage('init') {
    checkout scm
  }
  stage('build') {
      sh '''
      git pull origin master      
      git push azure master
      '''
   }  
}
