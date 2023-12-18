pipeline {

    agent {node { label 'workstation' }}
      options {
            ansiColor('xterm')
        }

    environment {
      SSH = credentials("SSH")
    }

    stages {
        stage ("Stage-1"){
            steps {
              echo "Hello world"
              sh 'env'
            }
        }
    }

    post {
      always {
        sh 'echo Build completed successfully'
      }
    }
}