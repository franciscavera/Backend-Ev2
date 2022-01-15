pipeline {
	agent any

	
stages{ 
    stage('Build'){
        steps{
            
            sh './gradle bootrun'
        }
    }

    stage('JUnit'){
            steps {
               
                       
						sh './gradle test'
                
            
		    }
        }
}


}
