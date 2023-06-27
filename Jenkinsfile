pipeline{
    agent any
    stages {
        stage('SSH & deploy'){
            steps {
               sh 'ssh node01 "docker stop myapp; docker rm myapp; docker run -d --name myapp -p 3000:3000 moshab679/myapp:1.0"'
            }
        }
    }
}
