node {
  withCredentials([usernameColonPassword(credentialsId: 'mylogin', variable: 'USERPASS')]) {
    sh '''
      set +x
      echo "$USERPASS" 
    '''
  }
}
