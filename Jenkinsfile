node {
    stage('Cloning Git Repo'){
        git branch: 'main', url: 'https://github.com/marlincia/jenkens-sonar.git'
    }
    stage('Scanning Code'){
       def scannerHome = tool 'SonarScanner';
       withSonarQubeEnv(InstallationName: 'Sonarqube') {
       sh "${scannerHome}/bin/sonar-scanner -Dsonar.projectKey=Sonar-jenkins"
      }
    }
}
