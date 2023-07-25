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
                 msbuild tool: 'MSBuild-5.0', projectFile: 'WEB.csproj', targets: 'Build', properties: [configuration: 'Release']
        
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

