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
		    <<EOT
DEP_ROOT='/home/matthewr/releases'
datestamp=$(date +%Y%m%d%H%M%S)
REL_DIR=$DEP_ROOT"/"$datestamp
if [ ! -d "$DEP_ROOT" ]; then
    echo "creating the root directory"
    mkdir $DEP_ROOT
fi
mkdir $REL_DIR
exit
EOT
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

 
