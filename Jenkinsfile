pipeline {  
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
		
	 post 
	  {
	    success
	     {
	     node('Production')
		 {
	               build job : 'ProdJob'
		 }
	     }	 
	  }
	}
     }
}     
