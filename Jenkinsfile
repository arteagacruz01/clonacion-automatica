pipeline {
    agent any
   
    stages {
        stage('credeciales') {
            steps {
                withCredentials([usernamePassword(credentialsId:'GIT', usernameVariable:"usuario", passwordVariable:"contrasena")]){
                script {
                     git branch: 'master', url: 'https://github.com/arteagacruz01/springboot.git'//, credentialsId: "${GIT}"
                }
                }
              
            }
        }
    }
        
    
}