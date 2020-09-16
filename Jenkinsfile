pipeline {
    agent any
    stages {
        stage ('Package Stage') {

            steps {
                 echo "compiling and packing"
                 bat label:'',script:'mvn package'    
            }
        }
        stage ('Testing Stage') {

            steps {
                echo "testing stage"
                  bat label:'',script:'mvn test'  
                }
        }
        stage ('Install Stage') {
            steps {
                echo "installing in local system"
                bat label:'',script:'mvn install' 
                    
                }
            }
        }
    }

