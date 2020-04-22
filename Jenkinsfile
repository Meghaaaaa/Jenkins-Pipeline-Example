pipeline{
  agent any
  
  stages{
    stage('Compile Stage'){
      
        steps{
        withMaven(maven: '3.6.3')
        {
          sh 'maven clean compile'
        }
     }
    }
     stage('Testing Stage'){
      
        steps{
        withMaven(maven: '3.6.3')
        {
          sh 'maven Test'
        }
     }
    }
     stage('Deployment Stage'){
      
        steps{
        withMaven(maven: '3.6.3')
        {
          sh 'maven Deploy'
        }
     }
    }
  }
}
