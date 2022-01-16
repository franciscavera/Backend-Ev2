pipeline {
	agent {label "newslave"}
    
    stages {

        stage('Hello'){
            steps {
			   
                sh '''
                java --version
                '''
		    }
        }
        stage("Pruebas unitarias"){
            steps{
                    dir("/var/lib/jenkins/workspace/demo2"){
                   
                    sh ''' ./gradlew test '''
        }
            }
        
    }

       
}
}