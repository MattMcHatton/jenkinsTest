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
