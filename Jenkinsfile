pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                withEnv(["KEY=sh 'python3 test.py'"] {
                    sh("python --version")
                    sh("echo Building..")
                    echo '${env.KEY}'
                    sh("echo $KEY")
                }
            }
        }
    }
}
