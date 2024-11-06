pipeline {
    agent {
        label 'java-label'
    }
    stages {
        stage('Build') {
           steps {
             retry(3){
                echo "welcome to jenkins pipeline"
                error "I will print error message"
             }
             echo "Message: After 3 times"
             
           } 
            
        }
    }
}
