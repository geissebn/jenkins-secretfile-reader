#!groovy
properties([parameters([string(description: 'credentials ID plz!', name: 'credentialsId', defaultValue: '')])])

node() {
  stage ('Reading credentials') {
    def id = params.credentialsId ?: 'foo'
    withCredentials([file(credentialsId: id, variable: 'CREDENTIALS_FILE')]) {
      checkout scm
      sh "cat $CREDENTIALS_FILE"
    }
  }
}
