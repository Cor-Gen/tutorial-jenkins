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
  agent { docker 'python:3.5.1' }
  stages {
    stage('build') {
      steps {
        sh 'pip --version'
        sh 'python --version'
      }
    }
  }
}
