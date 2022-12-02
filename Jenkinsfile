pipeline {
    agent { label 'OPENJDK-11-JDK' }
    stages {
        stage('learning') {
            steps {
                git url: 'https://github.com/longflewtinku/docker-1.git', 
                    branch: 'main'
            }
        }    
        stage('Example Build') {
            steps {
                sh 'docker image build -t two:1.0 .'  
            }
        }
    }
}