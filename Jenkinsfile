pipeline {
    agent any // Esegue su qualsiasi agente disponibile

    stages {
        stage('Checkout') {
            steps {
                checkout scm // Recupera il codice dal repository
            }
        }

        stage('Build') {
            steps {
                 echo 'building the project'
              
            }
        }

        stage('Test') {
            steps {
                echo ' testing the project '
            }
        }

        stage('Deploy') {
            steps {
                echo ' deploying the project'
            }
        }
    }
}
