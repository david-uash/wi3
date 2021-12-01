pipeline {
    agent {
                dockerfile true            
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
                    cat /tmp/helloFromDockerfile
                    cat /etc/passwd
                   '''    
            }
        }
    }
}
