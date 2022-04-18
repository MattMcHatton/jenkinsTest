pipeline {
    agent any

    stages {
        stage('Smoke Test') {
            steps {
                echo 'Building...'
                step('Smoke Test Environment UI'){
                    echo 'Smoke test...'
                }
            }
        }
        stage('Prepare') {
            steps {
                step('Prepare config file') {
                    echo 'Prepare config file...'
                }
                step('Remove existing reports') {
                    echo 'Removing existing reports...'
                }
            }
        }
        stage('Test') {
            steps {
                step('Running Maven Tests'){
                    echo 'Running maven tests'
                }
            }
        }
        stage('Archive'){
            steps {
                step('Publish Artifacts') {
                    echo 'Publishing artifacts...'
                }
                step('Insert Record into DB') {
                    echo 'Inserting records into DB...'
                }
            }
        }
    }
}