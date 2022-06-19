pipeline {    
    stages
    {
        stage('Hello')
	{
	  agent { label 'Test' }	
	   steps
	   {
	      echo "Hello World"
	   }
	}
	stage('GIT')
	{
	  steps
	  {
	    git 'https://github.com/Manjunathmba/JnekinsAssignment03.git'
	    
	  }
		
	 post 
	  {
	    success
	     {
	       build job : 'ProdJob'
	     }	 
	  }
	}
     }
}     
