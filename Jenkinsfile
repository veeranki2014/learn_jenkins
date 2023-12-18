pipeline {

    agent {node { label 'workstation' }}
      options {
            ansiColor('xterm')
        }

    environment {
      SSH = credentials("SSH")
    }

    parameters { string(name: 'APP_INPUT', defaultValue: '', description: 'JUST INPUT') }

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