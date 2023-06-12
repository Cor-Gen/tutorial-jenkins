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

  stage('SonarQube analysis') {
    echo "coucou"
    def scannerHome = tool 'SonarScanner 4.0';
//     withSonarQubeEnv('sq1') { // If you have configured more than one global server connection, you can specify its name
//       sh "${scannerHome}/bin/sonar-scanner"
//     }
  }
}

