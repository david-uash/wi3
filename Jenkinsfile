pipeline {
    agent { docker 
           { 
#               image 'python'
#               args '-u root' 
                dockerfile true
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
                    cat /root/helloFromDockerfile
                   '''    
            }
        }
    }
}
