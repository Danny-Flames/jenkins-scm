pipeline {
    agent any
    
    stages {
        stage('Checkout Code') {
            steps {
                echo 'Checking out repository...'
                checkout scm
            }
        }
        
        stage('Build') {
            steps {
                echo 'Building the project...'
                sh 'ls -la'  // Lists files in the workspace
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'cat index.html'  // Prints the content of index.html
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deployment stage (Not implemented yet)'
            }
        }
    }
    
    post {
        success {
            echo 'Build succeeded!'
        }
        failure {
            echo 'Build failed!'
        }
    }
}
