pipeline {
	agent any

    

    stages {

        stage('JUnit'){
            steps {
                
			    catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE') {
					dir("/var/lib/jenkins/workspace/BACKEND-EV2/demo2") {
						
                        sh './gradlew juniTest'
					}
                }
		    }
        }

     
}
}