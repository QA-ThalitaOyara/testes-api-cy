pipeline {
    agent any

    stages {
        stage('Clonar o repositorio') {
            steps {
                git branch: 'main', url: 'https://github.com/QA-ThalitaOyara/testes-api-cy.git'
            }
        }
    stage('Instalar dependencias') {
            steps {
            bat 'npm install'   
            }
        }
    stage('Executar testes') {
            steps {
            bat 'npm run cy:run'    
            }
        }
    }
}
