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
        fileExists 'bot2'
        sh '''#!/user/bin/env groovy

node {
  stage(\'Clone repository\') {
    // Clone the repository containing the Python code
    git \'https://github.com/PauGuiu/BOT2\'
  }

  stage(\'Read file\') {
    // Read the contents of the Python file
    def code = readFile(\'PauGuiu/BOT2.py\')

    // Print the contents of the file to the Jenkins console
    print code
  }

  stage(\'Create new file\') {
    // Write the contents of the original file to a new file
    writeFile file: \'PauGuiu/nuevo.py\', text: code
  }
}
'''
      }
    }

  }
}