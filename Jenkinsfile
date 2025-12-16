pipeline {
    agent any
    environment {
        PYTHON = 'C:\\Users\\hp\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe'
    }
    stages {
        stage('checkout code ') {
            checkout scm

        } 
          stages ('extract data') {
            bat :"${env.PYHTON} extract.py"
        }     
        
    }
    post {
        sucess {
            echo "sucess ...."

        }
        failure {
            echo "fail..."

       }
       always {
            echo "always..."
        }

    }   
}
