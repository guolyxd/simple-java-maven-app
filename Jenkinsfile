pipeline {
	agent
	{
	  docker {
	      image 'maven:latest'
	      sh 'echo "complete download images"'
	  }
	}
	stages {
	  stage ('Build'){
	     steps{
	       sh 'mvn -B -DskipTests clean package'
	     }
	  }
	}
}