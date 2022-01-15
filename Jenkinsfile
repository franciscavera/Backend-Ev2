pipeline {
	agent any

	
stages{ 

    stage('JUnit'){
            steps {
                script {
                   
                    catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE') {
                    		dir("/var/lib/jenkins/workspace/Backend-Ev2/demo2") 
						
                        bat './gradlew test'
                }
            }
		    }
        }
}


}
