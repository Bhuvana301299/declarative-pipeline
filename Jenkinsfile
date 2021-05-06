pipeline {
  agent any
  stages {
    stage('build') {
      agent any
      environment{
            LOGIC_LEVEL='INFO'
        }
      steps {
        echo "Building Release ${RELEASE} with log level ${LOG_LEVEL} ..."
      }
    }
    stage('Test'){
      steps{
        echo "Testing Release ${RELEASE} log level ${LOG_LEVEL} is not visible..."
      }
    }

  }
  environment {
    RELEASE = '20.05'
  }
}
