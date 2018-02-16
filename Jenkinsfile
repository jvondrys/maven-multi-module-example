pipeline {
  agent any
  stages {
    stage('init') {
      parallel {
        stage('init') {
          steps {
            echo 'Build zacina'
          }
        }
        stage('init2') {
          steps {
            sleep 5
          }
        }
      }
    }
    stage('build maven') {
      steps {
        sh 'mvn -B clean package'
      }
    }
  }
}