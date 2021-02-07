pipeline {
  agent any
   
   
   stages {
    stage('Build') {
      steps {
		    bat 'mvn -version'
			bat 'mvn clean install -DskipTests'
			
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
  