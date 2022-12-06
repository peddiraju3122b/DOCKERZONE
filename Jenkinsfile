pipeline{
    agent{ label 'node1'}
    stages{
        stage('DOCKER FILE'){
            steps{
                git url: 'https://github.com/peddiraju3122b/DOCKERZONE.git',
                branch: 'main'
            }
        }
        stage('image container'){
            steps{
                sh 'docker image build -t spc:1.0 .' 
                sh 'docker container run -d -P --name spc:1.0 /bin/sh -c'
                
            }
        }
    }
}