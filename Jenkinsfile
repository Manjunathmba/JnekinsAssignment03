pipeline {
  agent any 
    
    stages
    {
        stage('Hello')
	{
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
