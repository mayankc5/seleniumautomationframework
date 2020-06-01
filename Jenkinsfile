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
				step{
					bat label: '', script: 'set path=C:\\Program Files\\Java\\apache-maven-3.6.3\\bin'
				}
				step{
					bat label: '', script: 'mvn clean install'
				}
			}
		}
	}
}
