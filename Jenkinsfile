pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                git url: 'https://github.com/remaj94/szkolenie-ci-jenkins' , branch: 'main'
                dir('docker-pipeline') {
                script {
                    docker.build('myapp')
            }
                }        
        }
    }
}
}
