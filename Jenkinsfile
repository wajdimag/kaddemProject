pipeline {
    agent any
    tools {
        maven 'maven3'  // Make sure this matches the name in Global Tool Configuration
    }
    stages {
        stage('Checkout Code') {
            steps {
                checkout scm
            }
        }
        stage('Build with Maven') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
