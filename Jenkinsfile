pipeline {
  agent any
  stages {
    stage ("build") {
      steps {
        echo "building my app..."
        npm install
      }
    }
    stage ("test") {
       steps {
        echo "testing my app..."
        sh 'npm test'
       }
    }
    stage ("deploy") {
    steps {
        echo "deploying my app..."
        sh 'npm run dev'
       }
    }
  }

}