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
  post {
	always {
          echo 'This will always run' 
        }
	success {
          echo 'SUCCESS happend' 
        }	
	failure {
          echo 'Failed' 
        }
	unstable {
          echo 'Unstable' 
        }
	changed {
          echo 'Pipeline Changed' 
        }
  } 
}