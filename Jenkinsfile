@Library('shlib1')_
pipeline{
  agent any
  stages{
stage("NexusConnector"){
            steps{
             
       nexusconector()
              log_nexus("is executed")
        }
  post{
    failure{
      log_nexus("not executed")
        }
  }
}
    stage("NexusCollector"){
            steps{
             
       nexuscolector()
        }
        }
       
}
}
