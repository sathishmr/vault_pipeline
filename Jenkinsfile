pipeline {
    agent any
    environment {
        SECRET = vault path: 'secrets', key: 'username', vaultUrl: 'https://my-vault.com:8200', credentialsId: 'my-creds', engineVersion: "2"
    }
    stages {
        stage("read vault key") {
            steps {
                echo "${SECRET}"
            }
        }
    }
}
