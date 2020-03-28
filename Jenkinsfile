pipeline {
	agent any
	{
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

	  stage('Test'){

	  }

	  stage('Deploy'){
	  	
	  }
	  }
	}
}