pipeline {
    agent any
    stages {
        stage('build') {
            environment {
                KEY=sh(script: "python3 test.py", returnStdout: true)
            }
            steps {
                sh """
                set +x
                python --version
                python3 test.py
                python3 test.py
                echo $KEY
                set -x
                """
            }
        }
    }
}
