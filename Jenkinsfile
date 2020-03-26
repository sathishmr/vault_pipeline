node {
  withCredentials([usernameColonPassword(credentialsId: 'mylogin', variable: 'USERPASS')]) {
    sh '''
      set +x
      curl -u "$USERPASS" https://private.server/ > output
    '''
  }
}
