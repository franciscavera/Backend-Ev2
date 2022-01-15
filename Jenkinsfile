
pipeline{
      agent {label "newslave"}
      stages{

          stage('Hello'){
            stesps {
                sh '''
                java --version
                '''
            }
        }

        stage('Pruebas unitarias'){
            steps { 
            dir("/var/lib/jenkins/workspace/Tingeso/demo2"){
            sh ''' chmod +x ./gradlew '''
            sh ''' ./gradlew test '''}
        
        }
        }

      }
}
