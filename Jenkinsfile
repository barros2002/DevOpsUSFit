pipeline {
  agent any
  stages {
    stage('FetchLifeTimeData') {
      steps {
        powershell 'C:\\Users\\barros\\Desktop\\PowerShell\\FetchLifeTimeData.ps1'
      }
    }
    stage('DeployLatestTagsToTargetEnv') {
      steps {
        powershell 'C:\\Users\\barros\\Desktop\\PowerShell\\DeployLatestTagsToTargetEnv.ps1'
      }
    }
  }
  environment {
    LifeTimeUrl = 'https://pmdemo2-lt.outsystemsenterprise.com/'
    AuthorizationToken = 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJsaWZldGltZSIsInN1YiI6IllqTmpPRGRoWlRjdFlUSXhNaTAwTlRZekxUa3lOamt0TVRaak5qRmxOMk0yTWpObSIsImF1ZCI6ImxpZmV0aW1lIiwiaWF0IjoiMTU1MDgzNTA3OCIsImppdCI6ImVWenJQRmF4WlEifQ==.DRkxzotxSddJwk9l+1sGJDccHcnIyow1ZohypZiZ2zM='
  }
}