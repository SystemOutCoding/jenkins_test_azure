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
   stage('deploy') {
   azureWebAppPublish azureCredentialsId: env.AZURE_CRED_ID,
                       resourceGroup: env.RES_GROUP, appName: env.WEB_APP, filePath: "**/todo.zip"

  }
}
