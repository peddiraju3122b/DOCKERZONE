pipeline{
    agent{ lable "node1"}
    stages{
        stage("DOCKER FILE"){
            steps(git clone){
                giy url: "https://github.com/peddiraju3122b/DOCKERZONE.git"
                branch : "main"
            }
        }
        stage("image container"){
            steps(read,read and write layers creats){
                sh "docker image build spc:1.0"
                sh "docker image ls"
                sh "docker container run -d -it --name spc:1.0"
                
            }
        }
    }
}