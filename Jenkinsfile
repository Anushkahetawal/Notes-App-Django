@Library('Shared') _
pipeline{
    agent { label 'vinod'}
    
    stages{
        stage("Code Clone"){
            steps{
                script{
            clone("https://github.com/Anushkahetawal/Notes-App-Django.git","main")
                }
            }
        }
        stage("Code Build"){
            steps{
                script{
            docker_build("notes-app","latest","anushkahetawal")
                }
            }
        }
        stage("Push Image to DockerHub"){
            steps{
                script{
                docker_push("notes-app","latest","anushkahetawal")
                }
            }
        }
        stage("Deploy"){
            steps{
                script{
                docker_compose()
                }
            }
        }  
    }
}
