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
                sh 'pwd'
                sh 'cd'
                sh 'mkdir -p deleteme'
                sh 'pwd'
            }
        }
    }
}
