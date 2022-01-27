pipeline {
    agent any
    stages {
        stage('Make directory') {
            steps{
                sh 'mkdir ~/jenkins-tutorial-test'
            }
        }
        stage('Make files') {
            steps {
                sh 'touch ~/jenkins-tutorial-test/file1.txt'
                dir('~/jenkins-tutorial-test') {
                    sh 'touch file2.txt'
                }
            }
        }
    }
}
