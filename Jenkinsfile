node {
  stage ('SCM') {
    
  }
          
 stage 'Docker build' {
   docker.build('sample-nodejs-app')
 }
  

  stage 'Docker push'
  docker.withRegistry('https://676340509853.dkr.ecr.us-east-2.amazonaws.com', 'ecr:us-east-2:sample-nodejs-app-ecr-credentials') {
    docker.image('sample-nodejs-app').push('latest')
  }
}
