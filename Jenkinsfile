pipeline {
    agent any

    tools {
        nodejs "node" // Asegúrate que Jenkins tenga configurado este Node
    }

    stages {
        stage('Install') {
            steps {
                echo 'Instalando dependencias...'
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                echo 'Compilando la aplicación Angular...'
                sh 'npm run build'
            }
        }

        stage('Unit Tests') {
            steps {
                echo 'Ejecutando pruebas unitarias...'
                sh 'echo "No unit tests defined yet"'
            }
        }

        // Opcional si tienes pruebas E2E con Cypress o Protractor
        stage('E2E Tests') {
            steps {
                echo 'Ejecutando pruebas end-to-end...'
                sh 'npm run e2e'
            }
        }
    }
}
