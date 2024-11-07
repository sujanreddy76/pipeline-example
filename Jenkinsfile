pipeline {
    agent {
        label 'java-slave'
    }
    stages {
        stage('DockerBP'){
            steps {
                //nginx pull,change the name to myownname and push to my registry
                sh "docker pull nginx"
                // docker tag nginx sujanreddy76/nginx:b5
                // docker push sujanreddy76/nginx:b5

            }
        }
    }
}
