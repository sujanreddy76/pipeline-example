pipeline {
    agent {
        label 'java-label'
    }
    environment {
        DEPLOY_TO = 'production'
    }
    stages {
        stage('Build') {
            steps {
                echo 'building the project..'
            }
        }
        stage('sonar') {
            steps {
                echo 'running sonar scan..'
            }
        }
        stage('deploy to dev') {
            steps {
                echo 'deploying to dev'
            }
        }
        stage('deploy to qa'){
            steps {
                echo 'deploying to QA'
            }
        }
        stage('deploy to stage env'){
            when {
                expression {
                     BRANCH_NAME == /(production|staging|main)/
                }
            }
            steps {
                echo 'deploying to '
            }
        }
        stage('deploy to prod') {
            when {
                allOf {
                    branch 'prodbranch'
                    environment name: 'DEPLOY_TO', value: 'production'
                }
            }
            steps {
                echo 'deploying to prod'
            }
        }

    }
}
