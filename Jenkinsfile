pipeline {
    agent {
        label 'docker-slave'
    }
    environment {
        //key =value
        DOCKER_CREDS = credentials('dockerhub_creds') //username and password
    }
    stages {
        stage('DockerBP'){
            steps {
                echo "Deploying code in feature branch"

            }
        }
    }
}
