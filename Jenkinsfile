pipeline {
    agent {
       label 'java-slave'
    }
    parameters {
       string (name: 'PERSON', defaultValue: 'Sujan', description: 'Enter Your Name')
       choice (name: 'COURSE', choices: ['k8s', 'jenkins', 'docker'], description: 'Select the Course')
       booleanParam(name: 'CLOUD', defaultValue: true, description: 'Do you want to be certified in GCP?')

    }
    environment {
        CI_SERVER = 'Jenkins'
    }
    stages {
        stage('Firststage') {
            steps {
                 echo "Welcome ${params.PERSON}"
                 echo "You enrolled to ${params.COURSE}"
                 echo "You are certified in ${params.CLOUD}"
                 echo "You are using ${CI_SERVER}"

            }
        }
    }
}
