
pipeline{
    agent {label "newslave"}
    stages{
        stages('Hello'){
            stesps {
                sh '''
                java --version
                '''
            }
        }
    }
}