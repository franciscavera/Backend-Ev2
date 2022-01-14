pipeline {
	agent any

	

    stages {

        stage('JUnit'){
            steps {
			    catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE') {
					dir("/var/lib/jenkins/workspace/Backend-Ev2") {
			bat 'gradlew tasks'
						
                        bat 'gradlew test junitTest'
					}
                }
		    }
        }

       

        
}
}