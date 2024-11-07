pipeline {
    agent {
        label 'docker-slave'
    }
    stages {
        stage('DockerBP'){
            steps {
                //nginx pull,change the name to myownname and push to my registry
                sh "docker pull nginx"
                echo "***********Printing images before changing the tag*************"
                sh "docker images"
                sh "docker tag nginx sujanreddy76/nginx:b5"
                echo "***********Printing images after changing the tag*************"
                sh "docker images"
                echo "******pushing the image to repo******"
                sh "docker push sujanreddy76/nginx:b5"

            }
        }
    }
}
