pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh '''
                KEY=sh(script: "python3 test.py", returnStdout: true)
                echo $KEY
                set +x
                python --version
                echo $KEY
                set -x
                '''
            }
        }
    }
}
