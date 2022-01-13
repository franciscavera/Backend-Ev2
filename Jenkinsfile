pipeline {
	agent any

    

    stages {

        stage('JUnit'){
            steps {
                
			    catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE') {
					dir("/var/lib/jenkins/workspace/BACKEND-EV2/BACKEND-EV2") {
						
                        sh './gradlew test juniTest'
					}
                }
		    }
        }

     
}
}