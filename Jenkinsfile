pipeline {
	agent
	{
	  docker {
	      image 'maven:latest'
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