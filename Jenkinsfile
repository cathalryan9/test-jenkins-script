pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh """python --version
                echo Building..
                echo "bah"
                python3 test.py
                set +x
                python3 test.py
                echo $KEY
                """
            }
        }
    }
}
