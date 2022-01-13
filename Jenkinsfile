pipeline {
	agent any

	tools{
		gradle null
	}
    environment{
        DOCKERHUB_CREDENTIALS = credentials('franciscavera-dockerhub')
    }

    stages {

        stage('JUnit'){
            steps {
                cleanWS()
			    catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE') {
					dir("/var/lib/jenkins/workspace/BACKEND-EV2/demo2") {
						sh 'chmod +x ./gradlew'
                        sh './gradlew test'
					}
                }
		    }
        }

     
}
}