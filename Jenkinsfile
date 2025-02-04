pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from GitHub without credentials (since the repo is public)
                git url: 'https://github.com/wajdimag/kaddemProject.git', branch: 'patch-2'
            }
        }

        stage('Run Unit Tests') {
            steps {
                // Run unit tests (assuming you're using Gradle or Maven for building and testing)
                //sh './gradlew test'  // Use './mvn test' if you're using Maven instead of Gradle
            }
        }

        stage('Build Project') {
            steps {
                // Build the project (compile, package, etc.)
               // sh './gradlew build'  // Use './mvn package' if you're using Maven
            }
        }
    }
}
