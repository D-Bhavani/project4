pipeline {
    agent any


    tools {
        maven 'maven'
    }
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the source code from Git
                git 'https://github.com/D-Bhavani/project4.git'
            }
        }
        
        stage('Build') {
            steps {
                // Build the Java project using Maven
                sh 'mvn clean package'
            }
        }
        
        stage('Test') {
            steps {
                // Run tests using Maven
                echo 'mvn test'
            }
        }
    }
    
   
}
