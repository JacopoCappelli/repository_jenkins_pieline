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
                sh 'mvn clean install'
              sh 'npm install'
              
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                sh 'deploy.sh'
            }
        }
    }
}
