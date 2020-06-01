pipeline{
   agent any
	stages{
	
		stage('Build'){
		  steps{
			mvn clean install
		  }
		}
	
		stage('Test'){
		steps{
		
		    echo "Test sucessfull"
		  }
		}
		stage('Deployment'){
		steps{
		
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
