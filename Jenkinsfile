pipeline {
    agent {
        label 'java-label'
    }
    stages {
        stage('Build') {
            steps {
                echo 'building the project'
            }
        }
        stage('Scans') {
            parallel {
                stage('Sonar') {
                    steps {
                        echo 'running sonar scan'
                        sleep 10
                    }
                }
                stage('checkmarx') {
                    steps {
                        echo 'running checkmarx scan'
                        sleep 10
                    }
                }
                stage('fortify') {
                    steps {
                        echo 'running fortify scan'
                        sleep 10
                    }
                }
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy the project'
            }
        }
    }
}
