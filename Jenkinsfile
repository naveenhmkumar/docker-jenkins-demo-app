pipeline { 
    agent any 
    tools {
    maven 'M2_HOME'
  }
    stages { 
        stage('Build') { 
            steps { 
               echo 'This is a minimal pipeline.' 
                sh 'mvn --version'
                sh 'ssh -i .ssh/kumarhmweb'
                sh 'mkdri -p'
            }
        }
    }
}
