pipeline {
    agent any 
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/longnt890/CNPM.git'
            }
        }
        stage('Build') { 
            steps {
                echo 'Building..'
            }
        }
        stage('Test') { 
            steps {
                echo 'Testing..' 
            }
        }
        stage('Deploy') { 
            steps {
                echo 'Deploying..' 
            }
        }
    }
}

