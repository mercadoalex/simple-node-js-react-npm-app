pipeline {
    agent {
        docker {
            image 'node:lts-bulleye-slim'
            args: '-p 3000:3000'    
        } 
    }
    stages {
        stage('Build'){
            steps {
                sh 'npm install'
                echo "Construimos el proyecto JS"
            }
        }
        stage('Test'){
            steps {
                echo "Esta es la etapa de pruebas"
            }
        }
        stage('Staging'){
            steps{
                echo "Esta es la etapa de consolidacion" 
            }
        }     
    }
}
