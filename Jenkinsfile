pipeline {
    agent any
    stages {

        stage('test1') {
            when {
                changeset "**/test1/*.*"
            }
            steps {
            sh 'cat test1/test1.txt'
            }
        }
        stage('test2') {
            when {
                changeset "**/test2/*.*"
            }
            steps {
                echo 'building post trade'
            }
        }
    }
}
