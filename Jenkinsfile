pipeline {
  agent any
  stages {
    stage('install node') {
      steps {
        tool(name: 'nodejs', type: 'nodejs')
      }
    }

    stage('test') {
      steps {
        sh 'echo "start to build"'
        sh 'echo $PATH'
        sh 'node --version'
        sh 'sh build.sh'
      }
    }

  }
}