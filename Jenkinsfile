pipeline {
    agent any
    environment {
        SECRET = vault path: 'secrets', key: 'jenkins', vaultUrl: 'http://localhost:8200/', credentialsId: 'jenkins', engineVersion: "2"
    }
    stages {
        stage("read vault key") {
            steps {
                echo "${SECRET}"
            }
        }
    }
}
