pipeline{
    agent any
    stages{
        stage("Example_pipeline"){
            steps{
                script{
                    sh '''
                       ls -lrt
                       pwd
                    '''
                    
                }
                echo "example"
            }
  
        }
      stage("docker_build"){
        steps{
          script{
            sh '''
               sudo apt-get update 
                    sudo apt-get install -y docker.io
                    sudo systemctl start docker
                    sudo systemctl enable docker
                    docker --version
               '''
          }
        }
      }
        
    }
}
