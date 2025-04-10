pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Print hello.txt') {
            steps {
                script {
                    def content = readFile 'hello.txt'
                    echo "hello.txt says:\n${content}"
                }
            }
        }
    }
}
