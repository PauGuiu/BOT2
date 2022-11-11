pipeline {
  agent any
  stages {
    stage('paso 1') {
      steps {
        echo 'test1'
        build 'job1'
      }
    }

    stage('paso 2') {
      steps {
        mail(subject: 'a', body: 'a', to: 'pguiu@itbid.com')
      }
    }

  }
}