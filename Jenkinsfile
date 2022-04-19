pipeline {
    agent any

    stages {
        stage('Smoke Test') {
            steps {
                echo 'Smoke test...'
            }
        }
        stage('Prepare') {
            steps {
                echo 'Prepare config file...'
                echo 'Removing existing reports...'
                //bat should be used when running a script on Windows
                //sh should be used when running a script on Linux/Unix
            }
        }
        stage('Test') {
            steps {
                echo 'Running maven tests'
            }
        }
        stage('Archive'){
            steps {
                echo 'Publishing artifacts...'
                echo 'Inserting records into DB...'
            }
        }
    }
}
