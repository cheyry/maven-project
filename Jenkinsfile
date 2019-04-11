pipeline {
    agent any 
    stages {
        stage('Gitcheckout') { 
            steps {
                git credentialsId: 'githubid', url: 'https://github.com/cheyry/maven-project.git' 
            }
        }
        stage('Build') { 
            steps {
                sh """ mvn clean install -X """
            }
        }
        stage('Deploy') { 
            steps {
              sh """ echo "hello worlsk" """ 
            }
        }
    }
}