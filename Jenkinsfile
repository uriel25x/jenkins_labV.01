pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                sh 'bash scripts/hello.sh'
            }
        }

        stage('Build') {
            steps {
                sh 'bash scripts/build.sh'
            }
        }
    }
}
