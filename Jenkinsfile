pipeline {
  /*
   * TODO: Implement pipeline stages/steps
   *   See documentation: https://www.jenkins.io/doc/book/pipeline/syntax/#stages
   */
   agent any
   stages {
    stage('Build') {
        steps {
                sh './gradlew assemble'
                sh 'npm install -g yarn'
                sh 'yarn install'
            }
        }
    stage('Test') {
        steps {
            sh './gradlew test'
        }
    }
  }
}
