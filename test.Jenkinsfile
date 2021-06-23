pipeline {
    agent any
    environment { 
        KEY = ''
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                KEY=\$(python3 {WORKSPACE}/test.py)
            }
        }
    }
}
