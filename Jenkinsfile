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
                // sh 'ls'
                // sh 'cd ..'
                // sh 'ls'
                sh 'Write-Host \'Hello World!\''
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
