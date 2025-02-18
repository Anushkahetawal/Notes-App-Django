@Library('Shared')_
pipeline{
    agent { label 'vinod'}
    
    stages{
        stage("Code Clone"){
            steps{
            clone("https://github.com/Anushkahetawal/Notes-App-Django.git","main")
            }
        }
        stage("Code Build"){
            steps{
            docker_build("notes-app","latest")
            }
        }
        stage("Push Image to DockerHub"){
            steps{
                docker_push("dockerHubCreds","notes-app","latest")
            }
        }
        stage("Deploy"){
            steps{
                docker_compose()
            }
        }
        
    }
}
