#!/usr/bin/groovy

node {
  stage('scm'){
    resolveScm source: github(checkoutCredentialsId: 'SAME', id: '_', repoOwner: 'drbosse', repository: 'better-pipe'), targets: ['*']
  }
  stage('branch'){
    echo env.BRANCH_NAME
  }
}
