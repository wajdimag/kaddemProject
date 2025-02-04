pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from GitHub
                git credentialsId: '1cf28393-a127-4fc1-b458-bf1980e2c2e6', url: 'https://github.com/anis-saadouli/kaddemProject.git'
            }
        }

        stage('Run Unit Tests') {
            steps {
                // Run unit tests (assuming you're using Gradle or Maven for building and testing)
                sh './gradlew test'  // Use './mvn test' if you're using Maven instead of Gradle
            }
        }

        stage('Build Project') {
            steps {
                // Build the project (compile, package, etc.)
                sh './gradlew build'  // Use './mvn package' if you're using Maven
            }
        }
    }
}
