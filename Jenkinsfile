pipeline {
	agent any

	tools{
		gradle 'gradle-6.8.3'
	}
    environment{
        DOCKERHUB_CREDENTIALS = credentials('franciscavera-dockerhub')
    }
 stages {

      

        stage('Docker Build'){
            steps{
                dir("/var/lib/jenkins/workspace/backend/backend"){
                    sh 'docker build --build-arg JAR_FILE=build/libs/*.jar -t francisca/repo-back .'
                }        
            }
        }
       
        stage('Docker Hub'){
            steps{
                dir("/var/lib/jenkins/workspace/backend/backend"){
                    sh 'docker push franciscavera/repo-back'
                }
            }
        }
    }
    post{
        always{
            sh 'docker logout'
        }
    }
}