pipeline{
    agent{ label 'node1'}
    stages{
        stage('DOCKER FILE'){
            steps{
                git url: "https://github.com/peddiraju3122b/DOCKERZONE.git",
                branch: 'main'
            }
        }
        stage('image container'){
            steps{
                sh 'docker image build spc:1.0 .' \
                   '&& docker container run -d -it --name spc:1.0'
                
            }
        }
    }
}