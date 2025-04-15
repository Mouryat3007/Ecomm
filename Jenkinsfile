pipeline {
    agent any
    stages {
        stage ("Clone Repo") {
            steps{
                git branch: 'main', url: 'https://github.com/Mouryat3007/Ecomm.git'
            }
        }
        
        stage ('copy to var') {
            steps{
                script {
                    sh 'cp -r * /var/www/html'
                }
            }
        }
    }
}
