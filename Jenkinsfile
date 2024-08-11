pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build App'
            }
        }
         stage('Test') {
            steps {
                echo 'Test App'
            }
        }
         stage('Deploy') {
            steps {
                echo 'Dploy App'
            }
        }
    }
    
    post {
        always {
            
            emailext body: 'Pipeline Status for Reports', subject: 'Pipeline Status', to: 'lakhanchavan19031995@gmail.com'
        }
}

}
