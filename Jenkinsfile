pipeline{
    agent any
    environment {
        PATH = "$PATH:/opt/apache-maven-3.6.1/bin"
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
