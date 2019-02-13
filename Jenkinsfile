node {
  stage 'build'
  
  stage 'package'
  docker.build('naveenhm/nginx').push()

  stage 'deploy'
  sh './deploy.sh'
}
