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
                branch 'testing'
            }
            options {
                 retry 3
            }
            steps {
                echo "Deploying to ${deployEnv}"
            }
        }
    }
}
