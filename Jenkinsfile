pipeline{
 tools{
        jdk 'JAVA_HOME1'
        maven 'M2_HOME1'
    }
     agent { label 'winslave'}
	  
	  stages{
	  
	  stage("checkout"){
	   steps{
	   git 'https://github.com/ashisnishanka/maven-project-17.git'
	   }
	                  }
	  stage("compile"){
	   steps{
	      bat 'mvn compile'
	   }
	                  }
	 stage("test"){
	   steps{
	      bat 'mvn test'
	   }
	                  }
	stage("package"){
	   steps{
	      bat 'mvn package'
	   }
	                  }
	  
}
}
