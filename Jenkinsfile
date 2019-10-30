pipeline {
    agent { label 'master' }
    stages {
        stage('getCode') {
            steps {
                sh "mkdir -p hello-spring"
                dir('hello-spring') {
                    git branch: "master", url: "https://github.com/somir/hello-spring.git"
                }
            }
        }
    }
}
