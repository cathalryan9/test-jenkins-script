pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh """
                python --version
                python3 test.py
                set +x
                python3 test.py
                set -x
                """
            }
        }
    }
}
