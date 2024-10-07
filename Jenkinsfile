pipeline {
    agent any 

    environment {
        FLUTTER_HOME = '/Users/hari/Library/Flutter'
        PATH = "${FLUTTER_HOME}/bin:${env.PATH}"
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/haridev1004/cicd_pipeline_testing.git' // Replace with your repository URL
            }
        }

        stage('Install Dependencies') {
            steps {
                // Specify the shell directly
                sh 'flutter test'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'flutter test'
            }
        }

        stage('Build App') {
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
