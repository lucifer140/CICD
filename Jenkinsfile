pipeline {
    agent any

    stages {
       stage('build') {
           when {
               branch "next"
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
