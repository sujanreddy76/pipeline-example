pipeline {
    agent {
        label 'java-label'
    }
    tools {
        maven 'Maven_3.8.8' //This name should match to the name created under tool section
    }
    stages {
        stage('Build') {
            steps {
                echo "Welcome to tools demo"
                sh 'mvn --version'
            }
        }
    }
}
