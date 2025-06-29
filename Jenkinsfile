pipeline {
    agent { label 'apache' }

    stages {
        stage('Install Apache') {
            steps {
                sh '''
                    sudo apt update
                    sudo apt install -y apache2
                    sudo systemctl enable apache2
                    sudo systemctl start apache2
                    sudo systemctl status apache2
                '''
            }
        }
    }
}
