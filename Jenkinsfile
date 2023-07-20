// Steps: 

pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/betim009/PlayGround-Functions.git'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'npm install' // Instala as dependências do projeto
                sh 'npm test' // Executa o comando npm test
            }
        }
    }
}
