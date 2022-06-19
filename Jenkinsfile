pipeline {  
	agent {label 'Test'}
	options { skipDefaultCheckout() }
    stages
    {
	stage('TestJob')
	{
	  steps
	  {
	     checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'Manjunathmba', url: 'https://github.com/Manjunathmba/JnekinsAssignment03.git']]])
                sh "ls -lart ./*"
	    
	  }
	}
     }
}     
