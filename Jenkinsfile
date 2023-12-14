pipeline{
    agent any
    environment {
        PATH = "$PATH:C:\Program Files\apache-maven-3.8.6/bin"
    }
    stages{
	stage('GetCode'){
            steps{
		git branch: 'master',
                url: 'https://github.com/Devops142/maven-web-application-1.git'
            }
         }        
	stage('Build'){
            steps{
                sh 'mvn clean install'
            }
        }       
    }
}
