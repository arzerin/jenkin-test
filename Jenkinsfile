pipeline {
  agent any
  stages {
    stage('verify version') {
      steps {
        sh '/Applications/MAMP/bin/php/php8.1.1/bin/php --version'
      }
    }
    stage('hello') {
      steps {
        sh '/Applications/MAMP/bin/php/php8.1.1/bin/php hello.php'
      }
    }
  }
}