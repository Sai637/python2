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
               docker version
               '''
          }
        }
      }
        
    }
}
