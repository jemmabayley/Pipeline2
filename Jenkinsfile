pipeline {
    agent { any { image 'php' } }
    stages {
        stage('build') {
            steps {
                sh 'php --version'
                sh 'echo "Hello"'
                 sh 'mkdir archive1'
                sh 'echo test > archive1/test.txt'
                sh 'zip -r test.zip archive1'
                sh 'ls -las'
                archiveArtifacts artifacts: 'test.zip', onlyIfSuccessful: true
            }
        }
    }
}
