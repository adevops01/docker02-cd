pipeline{
    agent any
        stage('SSH & deploy'){
            steps {
               sh 'ssh node01 "docker stop nginx-container; docker rm nginx-container; docker run -d --name nginx-container -p 80:80 nginx:latest"'
            }
        }
    }
