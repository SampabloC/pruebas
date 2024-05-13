
// Jenkinsfile (Declarative Pipeline)

/* Requires the Docker Pipeline plugin */
pipeline {
    agent {
        docker {
            image 'ruby:3.3.1-alpine3.19'
            args '-v /var/run/docker.sock:/var/run/docker.sock'  // Esto monta el socket de Docker para acceso
        }
    }
    stages {
        stage('build') {
            steps {
                sh 'docker --version'  // Verifica que Docker esté disponible en el agente
            }
        }
    }
}

