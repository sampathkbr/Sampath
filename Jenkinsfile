pipeline {
    agent none
    stages {
        stage('scm'){
         steps
            git clone 'https://github.com/sampathkbr/Sampath.git/'
            cd Sampath
            sh docker build -t Sampath/dockernodejs .
            docker container run -it -p 8081:8080 -d --name nodeapplication Sampath/dockernodejs

        }
    }
}
