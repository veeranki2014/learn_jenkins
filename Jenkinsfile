pipeline {

    agent {node { label 'workstation' }}

    environment {
      SSH = credentials("SSH")
    }

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