pipeline {
	agent any

   tools {
    gradle "Gradle 6.8.3"
  }

	
stages {

       stage('JUnit'){
            steps {
			    catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE') {
					dir("/var/lib/jenkins/workspace/Backend-Ev2/demo2") {
						sh 'gradlew bootrun'
                        sh './gradlew test'
					}
                }
		    }
        }



}
}