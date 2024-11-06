pipeline {
    agent {
        label 'java-node'
    }
    stages {
        stage('Build'){
            steps {
                timeout (time: 5, unit: 'SECONDS') {
                    echo "Sleeping for 60 seconds"
                    sleep 60
                }
                
            }
        }
    }
}
