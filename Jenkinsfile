pipeline{
   agent any
	stages{
	
		stage('Build'){
		  steps{
		    mvn compile
		    echo "Build sucessfull"
		  }
		}
	
		stage('Test'){
		steps{
			mvn test
		    echo "Test sucessfull"
		  }
		}
		stage('Deployment'){
		steps{
		mvn package
		    echo "Deployment sucessfull"
		  }
		}
		stage('Release'){
		steps{
		    echo "Release sucessfull"
		  }
		}
	}


}
