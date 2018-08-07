pipeline{
  agent{
    label "windows"
   }

   tools{
    maven "apache-maven-3.5.2"
    jdk "jdk1.8.0_171"
   }
   stages{
			 stage('Initialize'){
				 steps{
					bat '''
					echo "PATH = $PATH"
					echo "M2_HOME = %M2_HOME%"
				   '''
				  }
			   }

			stage('test'){
				 steps{
					bat 'mvn install'
					
				  }
			   } 

			   stage('build'){
				 steps{
					bat 'mvn install'
					
				  }
			   } 
     } 
 
  }
