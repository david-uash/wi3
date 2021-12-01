pipeline {
    agent { docker 
           { 
               image 'python'
               args '-u root' 
           } 
          }
    environment {
        ACCKEY=credentials('ACCKEY')
        SECKEY=credentials('SECKEY')
    }
    stages {
        stage('build') {
            steps {
                sh '''
                    python --version
                   '''    
            }
        }
    }
}
