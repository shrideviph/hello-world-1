pipeline {
    agent any
    environment {
        PATH="/opt/maven/bin:$PATH"
    }

    stages {
        stage('SCM') {
            steps {
                git 'https://github.com/sekhareric/hello-world.git'
            }
        }
        stage('Maven') {
            steps {
                sh "mvn package"
            }
        }
        stage('hi') {
            steps {
                echo 'hi guys...!'
            }
        }
    }
}
