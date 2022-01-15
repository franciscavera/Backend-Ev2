pipeline {
	agent any

	
stages{ 
    stage('Build'){
        steps{
            dir("/var/lib/jenkins/workspace/Backend-Ev2/demo2") 
            sh './gradle assemble'
        }
    }

    stage('JUnit'){
            steps {
               
                        dir("/var/lib/jenkins/workspace/Backend-Ev2/demo2") 
						sh './gradle test'
                
            
		    }
        }
}


}
