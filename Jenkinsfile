pipeline {
  agent any
  stages {
    stage('first stage') {
      steps {
        git poll: true, url: 'https://github.com/arietan/jenkin-lab'
        echo 'Hello Jenkin pipeline!'
      }
    }
  }
}
