pipeline {
    agent {
        label 'java-label'
    }
    stages {
        stage('build') {
            steps {
                echo "Executing build block"
                sh 'hostname -i'
            }
        }
        stage('sonar') {
            steps {
                echo "Executiong sonar block"
            }   
        }
        // stage('docker') {
        //     agent {
        //         label 'docker-slave'
        //     }
        //     steps {
        //         sh 'docker pull nginx'
        //     }
        // }
    }
}
