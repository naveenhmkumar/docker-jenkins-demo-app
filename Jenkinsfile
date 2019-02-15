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
                sh 'sudo ssh -tt ec2-user@3.208.20.195'
                sh 'ls' 
            }
        }
    }
}
 
