pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/CTohQH/Hello-world-java2.git'
            }
        }
        stage('Build') {
            steps {

                        powershell 'gradle clean build'
                
            }
        }
        stage('Test') {
            steps {
                
                        powershell 'gradle test'
                  
            }
        }
        stage('Deploy') {
            steps {                
                        powershell 'java -jar build/libs/hello-world-java-V2.jar'
                 }           
        }
    
}


    }


