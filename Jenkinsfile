pipeline {
    agent none
    stages {
        stage('scm'){
         steps
            git clone 'https://github.com/sampathkbr/Sampath.git/'
            cd Sampath
            sh docker build -t dockernodejs .
            sh docker container run -it -p 8081:8080 -d  dockernodejs

        }
    }
}
