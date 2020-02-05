pipeline {
   agent any
   stages {
      stage('Deploy') {
         steps {
           bat '''
                cd demo-application
                dir
                kubectl apply -f deployment.yaml
                kubectl apply -f service.yaml
            '''
         } 
      }
      stage('Deploy Verification') {
         steps {
           bat '''
                // script to check log and exception patterns
                
            '''
         } 
      }
      stage('Functional/Integration testing') {
         steps {
           bat '''
               // to run the functional/Integration testcases
   
            '''
         } 
      }
      
      
      
   }
}
