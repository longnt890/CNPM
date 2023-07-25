pipeline {
    agent any 
    stages {
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
pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean install'
      }
    }
    stage('Deploy') {
      steps {
        sh 'cp target/*.war /opt/webserver/webapps'
      }
    }
  }
}
