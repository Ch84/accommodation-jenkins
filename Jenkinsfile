pipeline{
    
    agent any
    
    stages('Checkout'){
        
        steps{
            
            checkout scm
            
        }
    }
    // Bulding the web app
    
    stage('Build web-app'){
        
        steps{
            
            sh 'mvn -f /home/robot/.jenkins/workspace/test-jenkins-pipeline/hoteljsf clean install'
            
        }
    }
    // Building the web-service
    stage('Build web-service'){
        
        steps{
            
            sh 'mvn -f /home/robot/.jenkins/workspace/test-jenkins-pipeline/hotel-restfull clean install'
            
        }
     }    
  }
}

