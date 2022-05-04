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
        stage('deploy') {
            steps {
                sh '''
                docker run -d --name junkeys -p 7777:8080 jenks
                '''
            }
        }
        
    }
}
