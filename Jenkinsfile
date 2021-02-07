pipeline {
  agent any
   
   
   stages {
    stage('Build') {
      steps {
		    bat 'mvn -version'
			bat 'mvn -clean install -DskipTests'
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
  