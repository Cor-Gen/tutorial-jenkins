node {
  stage('SCM') {
    checkout scm
  }
  stage('sq1') {
    def scannerHome = tool 'SonarScanner';
    withSonarQubeEnv() {
      sh "${scannerHome}/bin/sonar-scanner"
    }
  }
}
}

