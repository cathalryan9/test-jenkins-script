pipeline {
    agent any
    environment { 
        KEY=\$(python3 test.py)
    }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'echo Building..'
                sh 'echo $KEY'
            }
        }
    }
}
