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
                sh 'msbuild WEBn.sln /p:Configuration=Release'
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

