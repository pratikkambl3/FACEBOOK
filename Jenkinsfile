pipeline{
	agent {
		label 'blue'
  		}
	stages{
		stage("Checkout scm"){
			steps{
				checkout scm
				}
			}
		stage("BUILD"){
			steps{
             sh '/home/grras/project/apache-maven-3.9.6/bin/mvn install'
			
}
	}
		stage("Deployment"){
			steps{
			sh ' scp target/FACEBOOK.war /home/pratikkambl3/Documents/Devops-Tools/apache-tomcat-9.0.89/webapps'		
		}
			}
		}
	
    	}
