pipeline {
  agent any

  stages {
    stage ("Deploy volumes"){
        steps {
            sh '''
            $kubectl apply -f ./volumes/
            '''
        }
    stage ("Deploy namespaces"){
      steps {
        sh '''
          $kubectl apply -f ./namespaces/
        '''
      }
    }
}
