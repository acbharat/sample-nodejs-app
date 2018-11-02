node {
  stage 'checkout'
  git 'https://github.com/acbharat/sample-nodejs-app'

  stage 'Docker Build'
  docker.build('sample-nodejs-app')
}