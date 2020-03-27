pipeline {
	agent {
	  docker {
	      image 'maven:3-alpine'
	      args '-u root --name test02  -v /root/.m2:/root/.m2'
	  }
	}
	stages {
	  stage ('build'){
	     steps{
	       sh 'mvn -B -DskipTests clean package'
	     }
	  }
	}
}