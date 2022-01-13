pipeline {
	agent any

    

    stages {

        stage('JUnit'){
            steps {
                
			    catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE') {
					dir("/var/lib/jenkins/workspace/build.gradle") {
						
                        sh 'gradlew test'
					}
                }
		    }
        }

     
}
}