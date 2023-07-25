pipeline {
    agent any 
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/longnt890/CNPM.git'
            }
        }
        stage('Build') { 
           script {
                    def msBuildVersion = 'MSBuild-5.0' // Replace with the name of the MSBuild installation configured in Jenkins
                    
                    // Execute MSBuild using the specified version
                    bat "\"${tool msBuildVersion}\" /t:Build /p:Configuration=Release WEB.csproj"
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

