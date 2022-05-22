pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                sh "cd /home/tur/DevOps/Jenkins"
                sh "sudo docker build -t 336869890/hwtura ."
                sh "sudo docker push 336869890/hwtura"
                


            }
        }
    }
}
