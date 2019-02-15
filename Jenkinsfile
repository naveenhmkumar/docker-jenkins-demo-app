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
                sh 'ssh -tt ec2-user@host1'
                sh 'ls' 
            }
        }
    }
}
 
