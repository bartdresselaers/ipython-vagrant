pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                retry(3) {
                    sh 'hostname'
                }

                timeout(time: 3, unit: 'MINUTES') {
                    sh 'df -kh'
                }
            }
        }
    }
}
