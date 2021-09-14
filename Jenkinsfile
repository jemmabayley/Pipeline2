pipeline {
    agent { any { image 'php' } }
    stages {
        stage('build') {
            steps {
                sh 'php --version'
                sh 'echo "Hello"'
                 sh 'mkdir archive'
                sh 'echo test > archive/test.txt'
                sh 'zip -r test.zip archive'
                sh 'ls -las'
            }
        }
    }
}
