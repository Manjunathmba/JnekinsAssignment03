pipeline {  
 agent any
    stages
    {
	stage('TestJob')
	{
		agent {label 'Test'}
	  steps
	  {
	    git 'https://github.com/Manjunathmba/JnekinsAssignment03.git'
	    
	  }
		
	 post 
	  {
            agent {label 'Production'}
	    success
	     {
	       build job : 'ProdJob'
	     }	 
	  }
	}
     }
}     
