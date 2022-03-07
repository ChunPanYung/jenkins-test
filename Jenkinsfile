pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'Hello World!'
                // sh 'mvn --version'
            }
        }
        stage('test') {
            steps {
                sh '''
                    #!/bin/env bash
                    echo "from bash script"
                '''
            }
        }
        stage('deploy') {
            steps {
                sh """
                    pwd
                    ls
                    chmod +x ./pudding.sh
                    sh ./pudding.sh
                """
            }
        }
    }
}
