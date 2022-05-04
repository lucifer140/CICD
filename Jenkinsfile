pipeline {
    agent any

    stages {
       stage('build') {
            steps {
                sh '''
               docker build -t jenks -f Dockerfile .
               docker images
               '''
            }
        }
        
    }
}
