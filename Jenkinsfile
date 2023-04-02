pipeline {
    agent any
    tools{
        maven 'MAVEN_HOME'
    }
    
    stages{
    
        stage('Build Maven'){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/KeralPatel3095/SpringBootCicd.git']]])
                bat 'mvn -X clean install'
            }
        }
        

	    
    }
    
}