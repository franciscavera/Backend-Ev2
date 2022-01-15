pipeline {
	agent any

	tools{
		gradle 'gradle-6.8.3'
	}

    stages {

        stage('JUnit'){
            steps {
                script {
                   
                    catchError(buildResult: 'SUCCESS', stageResult: 'FAILURE') {
                    		dir("/var/lib/jenkins/workspace/Backend-Ev2/demo2") 
						sh './gradle bootrun'
                        sh './gradlew test'
                }
            }
		    }
        }

       

        
}
}
