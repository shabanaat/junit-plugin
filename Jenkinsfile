pipeline { 
    agent any  
    stages { 
        stage('Build') { 
            steps { 
               echo 'This is a minimal pipeline.' 
            }
        }
		}
  
pipeline {
    agent any
    tools { 
        maven 'Maven 3.5.3' 
        jdk 'jdk8u162' 
    }
}
    stages {
        stage ('Initialize') {
            steps {
                sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                ''' 
            }
        }

        stage ('Build') {
            steps {
                echo 'This is a minimal pipeline.'
            }
        }
    
    }
	}
