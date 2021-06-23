pipeline {
    agent any
    environment { 
        KEY = ''
    }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'echo Building..'
                sh 'KEY=\$(python3 test.py)'
                sh 'echo $KEY'
            }
        }
    }
}
