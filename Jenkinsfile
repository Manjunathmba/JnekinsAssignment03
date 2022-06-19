pipeline {  
	agent {label 'Test'}
	options { skipDefaultCheckout() }
    stages
    {
	stage('TestJob')
	{
	  agent {label 'Test'}
	  steps
	  {
	     build job : 'TestJob'
	    
	  }
	}
     }
}     
