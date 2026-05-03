pipeline {
    agent any

    stages {
        stage('Pull Code') {
            steps {
                echo 'Code pulled from GitHub'
            }
        }

        stage('Show File') {
            steps {
                bat 'type index.html'
            }
        }

        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
    }
}