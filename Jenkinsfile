// pipeline {
//     agent { node { label 'docker-agent-alpine' } }
//     stages {
//         stage('build') {
//             steps {
//                 echo "Build stage from pipeline"
//             }
//         }
//     }
// }

node {
  stage('sq1') {
    def scannerHome = tool 'SonarScanner 4.0';
    withSonarQubeEnv('My SonarQube Server') { // If you have configured more than one global server connection, you can specify its name
      sh "${scannerHome}/bin/sonar-scanner"
    }
  }
}
