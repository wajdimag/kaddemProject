node {
  stage('Checkout Code') {
    checkout scm  // Pull code from the repository
  }

  stage('Build with Maven') {
    sh 'mvn clean install'  // Maven build command
  }
}
