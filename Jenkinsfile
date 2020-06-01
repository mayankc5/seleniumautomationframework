pipeline{
   agent any
	stages{
		stage('checkout'){
		  steps{
		      checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/mayankc5/seleniumautomationframework.git']]])
		     
		   }
		}
		stage('test'){
			steps{
			bat label: '', script: 'mvn clean install'
			}
		}
	}
}
