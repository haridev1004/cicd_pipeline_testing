pipeline {
    agent any 
    environment {
        PATH = "$PATH:/Users/hari/Library/Flutter/bin"
    }

      stages {
        stage('Setup') {
            steps {
                print "${env.PATH}"
            }    
        }
        
        stage('Build') {
            steps {
                sh "flutter doctor -v"
            }
        }        
    
    }
}

 
