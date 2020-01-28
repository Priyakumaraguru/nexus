@Library('shlib')_
pipeline{
  agent any
  stages{
stage("NexusConnector"){
            steps{
              withCredentials([usernamePassword(credentialsId: 'nexus_Credentials')])
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
