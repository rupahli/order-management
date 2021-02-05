pipeline {
  agent any
  
  stages {
    stage('Build') {
      steps {
			sh 'mvn -version'
			sh 'mvn clean install -DskipTests'
      }
    }
	}
	 post {
		always {
			echo 'build success'
            /*cleanWs()*/
        }
  }
}
  