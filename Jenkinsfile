pipeline {
    agent {
        label 'java-label'
    }
    stages {
        stage ("Hello") {
            steps {
                 //actual steps
                 echo "hello world"
                 sh 'date'
                 echo "executing my first stage"
                 sh 'sleep 10'
            }
           
        }
    
    stage('scriptblock') {
        steps {
            script {
                //my script
                //define a variable
                def course = "k8s"
                if(course == "k8s")
                    println("Thanks for enrolling in ${course}")
                    //${variable} , ${env.variable}
                else
                  println("Do learn ${course}")
                  sleep 20 // this sleep 20 is equal to (sh 'sleep 20').
            }
        }
     }
   }
}
