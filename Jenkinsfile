pipeline {
    agent any

    stages {

        stage('Deploy to Kubernetes') {
            steps {
                bat 'kubectl apply -f k8s/'
            }
        }

        stage('Check Pods') {
            steps {
                bat 'kubectl get pods'
            }
        }
    }
}
