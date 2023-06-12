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

pipeline {
withSonarQubeEnv('sq1', envOnly: true) {
  // This expands the evironment variables SONAR_CONFIG_NAME, SONAR_HOST_URL, SONAR_AUTH_TOKEN that can be used by any script.
  println ${env.SONAR_HOST_URL} 
}
}
