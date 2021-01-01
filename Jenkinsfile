// Uses Declarative syntax to run commands inside a container.
pipeline {
    agent {
        kubernetes {
            yamlFile 'pod.yaml'
            defaultContainer 'nodejs'
        }
    }
    stages {
        stage('Main') {
            steps {
                sh 'node --version'
            }
        }
    }
}
