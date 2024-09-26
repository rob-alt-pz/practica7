pipeline {
    agent any
    stages {
      stage('Checkout') {
        steps {
          git 'https://github.com/<nombre del repositorio>.git'
        }
      }
      stage('Install Dependencies') {
        steps {
          script {
            echo 'Installing dependencies...'
            sh 'npm install'
          }
        }
      }
    stage('Run Tests') {
      steps {
        script {
          echo 'Running tests...'
          sh 'npm test'
        }
      }
    }
    stage('Build') {
      steps {
        script {
          echo 'Building the application...'
          // Agregar cualquier paso de construcción necesario
        }
      }
    }
  }
}
