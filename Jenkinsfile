pipeline{
 tools{
        jdk 'Java_home'
        maven 'Maven_Home'
    }
     agent any
	  
	  stages{
	  
	  stage("checkout"){
	   steps{
	   git 'https://github.com/ashisnishanka/maven-project1.git'
	   }
	                  }
	
	   stage("compile"){
	    steps{
		 sh 'mvn compile'
		}
		}
		stage("test"){
	    steps{
		 sh 'mvn test'
		}
		}
		stage("package"){
	    steps{
		 sh 'mvn package'
		}
		}
	  }
	}
