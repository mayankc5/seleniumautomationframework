pipeline{
   agent any
	tools {
        maven 'Maven' 
    }
	stages{
		stage('checkout'){
		  steps{
		      checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/mayankc5/seleniumautomationframework.git']]])
		     
		   }
		}
		
		stage('compile'){
			steps{
				bat label: '', script: 'mvn compile'
				}
			
		}
		stage('verify'){
			steps{
				bat label: '', script: 'mvn verify'
				}
			
		}
		stage('test'){
			steps{
				bat label: '', script: 'mvn clean install'
				}
			
		}
	}
}
