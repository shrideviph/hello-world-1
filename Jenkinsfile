pipeline {
    agent any
    environment {
        PATH="/opt/maven/bin:$PATH"
    }

    stages {
        
        stage('SCM') {
            steps {
                git branch: 'master', url: 'https://github.com/sekhareric/hello-world.git'
            }
        }
        stage('Maven') {
            steps {
                sh "mvn clean package"
            }
        }
    }
}
