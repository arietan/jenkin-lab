pipeline {
  agent any
  stages {
    stage('Clone repo') {
      steps {
        git poll: true, url: 'https://github.com/arietan/jenkin-lab'
      }
    }
    stage('Package') {
      steps {
      	sh 'chmod +x package.sh'
        sh './package.sh'
      }
    }
    stage('Upload to S3') {
    	steps {
    		echo 'Upload to S3'
    	}
    }
  }
}
