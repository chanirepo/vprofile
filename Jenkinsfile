pipeline{
  agent any
  tools {
    maven "maven"
  }
  stages{

  stage('CheckOutCode'){
    steps{
   git 'https://github.com/chanirepo/vprofile.git' 
	}
  }
	  stage[build] {
		  steps {
			  sh "mvn clean package"
		  }
	  }
    }
  }
