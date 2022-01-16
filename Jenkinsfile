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
                    dir("/home/ubuntu/workspace/pruebaFran "){
                   
                    sh ''' ./gradlew test '''
        }
            }
        
    }

       
}
}