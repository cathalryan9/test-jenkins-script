pipeline {
    agent { docker { image 'python:3.5.1' } }
    environment { 
        KEY = ''
    }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'echo Building..'
                sh 'KEY=\$(python3 {WORKSPACE}/test.py)'
                sh 'echo $KEY'
            }
        }
    }
}
