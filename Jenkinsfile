pipeline {
    agent {
        label 'java-slave'
    }
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage('Build') {
            when {
                environment_name: 'DEPLOY_TO', value: 'production'
            }
            steps {
                echo 'building the project..'
            }
        }
    }
}
