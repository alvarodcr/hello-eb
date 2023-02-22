def AWS_KEY_ROOT = '2934977b-3b53-4065-8b4a-312c2259a9f3'		// AWS credentials for creating instances

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
