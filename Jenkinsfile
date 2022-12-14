pipeline {
  agent any
  stages {
    stage('paso 1') {
      steps {
        echo 'test1'
      }
    }

    stage('paso 2') {
      steps {
        mail(subject: 'aaa', body: 'aaa', to: 'pguiu@itbid.com', from: 'pguiu@itbid.com')
      }
    }

  }
}