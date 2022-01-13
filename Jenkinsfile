pipeline {
	agent any

    

    stages {

        stage('JUnit'){
            steps {
                
			    catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE') {
					dir("/var/lib/jenkins/workspace/Backend-Ev2/build.gradle") {
						
                        sh './gradlew test junitTest'
					}
                }
		    }
        }

     
}
}