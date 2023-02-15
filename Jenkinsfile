node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    def mvn = tool 'Default Maven';
    withSonarQubeEnv(instalationName: 'sonar') {
      sh "${mvn}/bin/mvn clean test sonar:sonar -Dsonar.projectKey=jenkins"
    }
  }
}
