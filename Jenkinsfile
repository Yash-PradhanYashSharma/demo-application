pipeline {
   agent any
   stages {
       stage('Clean-up') {
         steps {
            
            echo "Cleaning up the workspace" 
         }
      }
      stage('Git Clone') {
         steps {
            
            git  "https://github.com/Yash-PradhanYashSharma/demo-application.git"
            
         }
      }

      stage('Deploy') {
         steps {
           bat '''
                cd demo-application
                dir
                kubectl version
                kubectl --kubeconfig config apply -f deployment.yaml 
                kubectl --kubeconfig config apply -f service.yaml
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
