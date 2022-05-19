pipeline {
    agent none
    stages {
        stage('scm'){
         steps
            sh git clone 'https://github.com/sampathkbr/Sampath.git/'
            sh cd Sampath
            sh docker build -t dockernodejs .
            sh docker container run -it -p 8081:8080 -d  dockernodejs
        }
    }
}
