pipeline{
    agent any

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
