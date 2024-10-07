pipeline {
    agent any 
    
    environment {
        FLUTTER_HOME = '/Users/hari/Library/Flutter' // Set your Flutter SDK path
        PATH = "${env.FLUTTER_HOME}/bin:${env.PATH}" // Update PATH
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/haridev1004/cicd_pipeline_testing.git' // Replace with your repository URL
            }
        }


        stage('Run Tests') {
            steps {
                sh 'flutter test'
            }
        }

        
    }

    post {
        success {
            echo 'Build completed successfully!'
        }
        failure {
            echo 'Build failed!'
        }
    }
}
