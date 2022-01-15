pipeline {
	agent any

	
stages{ 
    stage('Build'){
        steps{
            dir('./Backend-Ev2/demo2')
            sh './gradle bootrun'
        }
    }

    stage('JUnit'){
            steps {
               
                        dir(./Backend-Ev2/demo2')
						sh './gradlew test'
                
            
		    }
        }
}


}
