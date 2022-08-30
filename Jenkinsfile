pipeline {
    agent any
    
    environment {
        unique_Id = UUID.randomUUID().toString()
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                snDevOpsChange()
                echo 'Completed change step...'
                echo 'Deploying....'
            }
        }
    }
}
