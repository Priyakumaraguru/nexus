@Library('shlib1')_
pipeline{
  agent any
  stages{
stage("NexusConnector"){
            steps{
             
       nexusconector()
        }
        }
        stage("NexusCollector"){
            steps{
       nexuscollector()
        }
        }
}
}
