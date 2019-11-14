pipeline {
<<<<<<< HEAD
    agent {
        docker {
            image 'maven:3-alpine'
            args '-v /root/.m2:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
            }
        }
        stage('Test') { 
            steps {
                sh 'mvn test' 
            }
            post {
                always {
                    junit 'target/surefire-reports/*.xml' 
                }
            }
        }
    }
=======
  agent any
  stages {
    stage('build') {
      steps {
        sh 'docker logs -f jenkins'
      }
    }

  }
>>>>>>> adb88bc10c168eb3c649d36c7ab8e0bd0fa01230
}