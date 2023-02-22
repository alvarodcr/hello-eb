pipeline {
	
    agent any 
    options {
        timestamps()
        ansiColor('xterm')
    }
	
    stages {
        
	stage('DOCKER --> BUILDING & TAGGING IMAGE') {
            steps{
		dir("hello-eb-files"){
		    withAWS(credentials:AWS_KEY_ROOT) {
		        sh "eb deploy"
		
		    }
		}
            }
        }   
    
    }
}
