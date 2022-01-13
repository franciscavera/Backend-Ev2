pipeline {
	agent any

    

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