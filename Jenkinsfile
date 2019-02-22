pipeline {
  agent any
  stages {
    stage('GetOAP') {
      steps {
        sleep 1
      }
    }
    stage('FetchLifeTimeData') {
      steps {
        powershell 'C:\\Users\\barros\\Desktop\\PowerShell\\FetchLifeTimeData.ps1'
      }
    }
  }
}