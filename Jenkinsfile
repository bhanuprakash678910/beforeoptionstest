pipeline {
    agent none
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Example Deploy') {
            when {
                beforeOptions true
                branch 'master'
            }
            options {
                 retry 3
            }
            steps {
                echoo "Deploying to master"
            }
        }
    }
}
