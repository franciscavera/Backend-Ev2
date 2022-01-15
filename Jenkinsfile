pipeline {
	agent any

	
stages{ 
    stage('Unit & Integration Tests') {
            steps {
                script {
                    try {
                        sh './gradlew clean test --no-daemon' //run a gradle task
                        sh './gradlew test'
                    } 
                }
            }
        }
}


}
