node {
  stage('build'){
    echo ' Image is building man'
  }
  
  stage('package'){
  docker.build('kohsuke/acmecorp-app').push()
  }
  stage 'deploy'
  sh './deploy.sh'
}
