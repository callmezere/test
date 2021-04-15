pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'app.py'
            }
        }
        stage('Test') {
            steps {
                echo 'app.py'
            }
        }
               stage('Deploy') {
                    steps {
                        echo 'app.py'
         }
     }
}

post {
        success {
            echo 'Build success'
            sh 'curl -d "chat_id=-492035825&text=Build success" https://api.telegram.org/bot1791406178:AAELmFtaFgaMCPV1yfCmBryDtrGqFhc0faw/sendMessage?chat_id=-492035825&text=Build'
        }
        
        failure {
            echo 'Build Automation'
            sh 'curl -d "chat_id=-492035825&text=Build Success" https://api.telegram.org/bot1791406178:AAELmFtaFgaMCPV1yfCmBryDtrGqFhc0faw/sendMessage?chat_id=-492035825&text=Success'
        }
    }
}
