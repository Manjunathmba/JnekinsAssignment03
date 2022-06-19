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
