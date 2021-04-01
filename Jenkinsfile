pipeline {
    agent { label 'slave-node'}
    stages {
        stage("nodejs") {
            steps {
                sh '''git clone https://github.com/quangtan191/jenkins.git
                cd /root/test_github/nodejs-todolist/nodejs-todolist
                docker build -t nodejs-todo:v3 .'''
            }
        }
    }
}
