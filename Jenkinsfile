pipeline {
    agent any
    stages {
        stage('build') {
            environment { 
                KEY=sh(script: "python3 test.py", returnStd)
            }
            steps {
                sh("python --version")
                sh("echo Building..")
                echo '${env.KEY}'
                sh("echo $KEY")
            }
        }
    }
}
