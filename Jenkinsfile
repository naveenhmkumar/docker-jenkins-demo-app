node {
  stage('build'){
    echo ' Image is building man'
  }
  
  stage('package'){
  docker.build('naveenhm/nginx').push()
  }
  stage 'deploy'
  sh './deploy.sh'
}
