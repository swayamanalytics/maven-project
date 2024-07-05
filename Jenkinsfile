pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
      withMaven(maven : 'localMaven'){
         sh 'mvn clean compile'
      }
    
    }
    }
    stage('Package Stage') {
      steps {
      withMaven(maven : 'localMaven'){
	 sh 'mvn clean package'
      }

    }
  }
}
