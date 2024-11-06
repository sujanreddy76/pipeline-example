pipeline {
    agent {
        label 'java-label'
    }
    environment {
       NAME = "siva"
       COURSE ="k8s"
    }
    stages {
        stage('Build') {
            environment {
                CLOUD = "GCP"
            }
            steps {
                echo "Welcome ${NAME}"
                echo "you are enrolled to ${COURSE} course"
                echo "you are certified in ${CLOUD}"
            }
        }
       stage('FirstStage') {
            
            steps {
                echo "Welcome ${NAME}"
                echo "you are enrolled to ${COURSE} course"
                echo "you are certified in ${CLOUD}"
            }
        }
    }
}
