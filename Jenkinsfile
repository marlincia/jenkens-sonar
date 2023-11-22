pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git(url: 'https://github.com/marlincia/jenkens-sonar', branch: 'main')
            }
        }
    }
}
