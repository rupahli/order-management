pipeline {
  agent any
   
  stages {
  stage ('Initialize') {
            steps {
                bat '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                ''' 
            }
        }
		
    stage('Build') {
      steps {
	  echo 'build success1'
			bat 'mvn -version'
			echo 'build success111'
			bat "C:\\Users\\ankit\\Documents\\Rupahli\\tools\\apache-maven-3.6.3-bin\\apache-maven-3.6.3\\mvn" -version
			echo 'build success2'
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
  