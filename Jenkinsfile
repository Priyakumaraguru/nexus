@Library('shlib1')_
pipeline{
  agent any
  stages{
stage("NexusConnector"){
            steps{
             
       nexusconector()
              log_nexus("is created successfully")
        }
  post{
    failure{
      log_nexus("is not created")
        }
  }
}
    stage("NexusCollector"){
            steps{
             
       nexuscolector()
               log_nexus("is listed successfully")
        }
  post{
    failure{
      log_nexus("does not exist")
        }
  }
        }
        
    stage("Nexus status"){
            steps{
             
       nexus_status()
              log_nexus("is created successfully")
        }
  post{
    failure{
      log_nexus("is not created")
        }
  }
}   
}
}
