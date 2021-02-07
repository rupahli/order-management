pipeline {
  agent any
   
   
   stages {
    stage('Build') {
      steps {
			bat 'C:\\Users\\ankit\\Documents\\Rupahli\\tools\\apache-maven-3.6.3-bin\\apache-maven-3.6.3\\bin\\mvn' -version
			bat 'C:\\Users\\ankit\\Documents\\Rupahli\\tools\\apache-maven-3.6.3-bin\\apache-maven-3.6.3\\bin\\mvn' clean install -DskipTests
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
  