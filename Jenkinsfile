pipeline {

    agent node {node { label 'workstation' }}

    stages {
        stage ("Stage-1"){
            steps {
              echo "Hello world"
            }
        }
    }

    post {
      always {
        sh 'echo Build completed successfully'
      }
    }
}