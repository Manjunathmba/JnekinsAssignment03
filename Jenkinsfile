pipeline {  
	agent {label 'Test'}
	options { skipDefaultCheckout() }
    stages
    {
	stage('TestJob')
	{
	  steps
	  {
	     checkout([$class: 'GitSCM', branches: [[name: '*/develop']], extensions: [], userRemoteConfigs: [[credentialsId: 'git-credentials', url: 'https://github.com/Manjunathmba/JnekinsAssignment03.git']]]
                sh "ls -lart ./*"
	    
	  }
	}
     }
}     
