pipeline {
    agent any
    stages {
        stage ('Workspace Cleanup') {
          cleanWs()                              
        }
        stage('test1') {
            when {
                changeset "**/test1/*.*"
            }
            steps {
                
                echo 'building match engine'
                cat test1/test1.txt
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
