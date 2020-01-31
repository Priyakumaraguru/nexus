@Library('shlib1')_
pipeline{
  agent any
  stages{
stage("NexusConnector"){
            steps{
             
       nexusconector()
              log_nexus("Repo created successfully")
        }
  post{
    failure{
      log_nexus("Repo is not created")
        }
  }
}
    stage("NexusCollector"){
            steps{
             
       nexuscolector()
               log_nexus("Repo is listed successfully")
        }
  post{
    failure{
      log_nexus("Repo does not exist")
        }
  }
        }
        
       
}
}
