pipeline {
    agent any

    stages {
       stage('build') {
           when {
               branch "develop"
           }
            steps {
                sh '''
               docker build -t jenks -f Dockerfile .
               docker images
               '''
            }
        }
        
    }
}
