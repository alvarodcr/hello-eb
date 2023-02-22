pipeline {
	
    agent any 
    options {
        timestamps()
        ansiColor('xterm')
    }
	
    stages {
        
	stage('DOCKER --> BUILDING & TAGGING IMAGE') {
            steps{
		dir ("hello-eb-files"){
		    sh "eb deploy"
		}
		
            }
        }   
    
    }
}
