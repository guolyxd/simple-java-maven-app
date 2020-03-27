pipeline {
	agent {
	  docker {
	      image 'maven:latest'
	      //args '-v /root/.m2:/root/.m2'
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