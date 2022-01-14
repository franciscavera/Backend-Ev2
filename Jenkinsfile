pipeline {
	agent any

	tools{
		gradle 'gradle-6.3'
	}

    stages {

        stage('JUnit'){
            steps {
                script {
                    try {
                        sh './gradlew clean test --no-daemon' //run a gradle task
                    } finally {
                        junit '**/build/test-results/test/*.java' //make the junit test results available in any case (success & failure)
                    }
                }
            }
		    }
        }

       

        
}
}