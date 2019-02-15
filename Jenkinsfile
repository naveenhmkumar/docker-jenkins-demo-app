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
                sh 'ls' 
                sh 'ssh -i kumarnhmweb  -T ec2-user@172.31.22.138'
		    sh 'ls'
                sh 'ls -al'
                sh 'exit'
                sh 'exit'
                sh 'ls -al'
                
            }
	    }
        stage('deploy'){
                steps {
                  sh 'ls'
                }
            }
    }
}

 
