pipeline {
	agent {
	  docker {
	      image 'maven:latest'
	      args '-u root'
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