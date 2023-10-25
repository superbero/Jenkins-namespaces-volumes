pipeline {
  agent any

  stages {
    stage ("Deploy volumes"){
        steps {
            sh '''
            $kubectl apply -f namespaces_volumes/namespaces
            '''
        }
    }
    stage ("Deploy namespaces"){
      steps {
        sh '''
          $kubectl apply -f namespaces_volumes/namespaces/
        '''
      }
    }
  }
}
