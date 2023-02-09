pipeline {
    agent any
    environment {
        PATH="/opt/apache-maven-3.9.0/bin:$PATH"
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
          stage('build') {
            steps {
                git 'https://github.com/manjunaik07/hello-world.git'
            }   
        }
         stage('mvn') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
