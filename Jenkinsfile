pipeline {
  agent any
   tools { 
        maven 'Maven 3.6.3' 
        jdk 'jdk8' 
    }
  
  stages {
  stage ('Initialize') {
            steps {
                sh '''
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
  