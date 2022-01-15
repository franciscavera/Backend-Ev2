pipeline {
	agent any

	
stages{ 
    stage('Build'){
        steps{
            
            sh './gradle assemble'
        }
    }

    stage('JUnit'){
            steps {
               
                        dir('./Backend-Ev2/demo2')
						sh './gradle test'
                
            
		    }
        }
}


}
