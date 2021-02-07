pipeline {
  agent any
   
    stage('Build') {
      steps {
	  echo 'build success1'
			echo 'build success111'
			bat "C:\\Users\\ankit\\Documents\\Rupahli\\tools\\apache-maven-3.6.3-bin\\apache-maven-3.6.3\\bin\\mvn" -version
			bat "C:\\Users\\ankit\\Documents\\Rupahli\\tools\\apache-maven-3.6.3-bin\\apache-maven-3.6.3\\bin\\mvn" -clean install -DskipTests
			echo 'build success2'
      }
    }
	
	 post {
		always {
			echo 'build success'
            /*cleanWs()*/
        }
  }
}
  