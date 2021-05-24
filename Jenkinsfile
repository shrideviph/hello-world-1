pipeline {
    agent any
    environment {
        PATH="/opt/maven/bin:$PATH"
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('SCM') {
            steps {
                git 'https://github.com/sekhareric/hello-world.git'
            }
        }
        stage('Build') {
            steps {
                sh "mvn clean package"
            }
        }
    }
}
        
