pipeline {
    agent { label 'slave-node'}
    stages {
        stage("nodejs") {
            steps {
                sh '''git clone https://github.com/quangtan191/jenkins.git
                cd nodejs-todolist
                docker build -t nodejs-todo:v3 .'''
            }
        }
    }
}
