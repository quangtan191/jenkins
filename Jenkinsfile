pipeline {
    agent { label 'slave-node'}
    stages {
        stage("nodejs") {
            steps {
                git 'https://github.com/quangtan191/jenkins.git'
            }
        }
        stage("build") {
            steps {
		sh '''cd jenkins
		docker build -t nodejs-todo:v4 .'''
            }
        }
    }
}
