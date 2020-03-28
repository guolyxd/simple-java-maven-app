pipeline {
	agent
	{
	  docker {
	      image 'maven:latest'
	      args 'docker run -it --rm --name my-maven-project -v "$(pwd)":/usr/src/mymaven -w /usr/src/mymaven maven:latest mvn clean install'
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