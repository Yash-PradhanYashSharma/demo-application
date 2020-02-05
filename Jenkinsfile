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
                kubectl apply -f deployment.yaml --token ZXlKaGJHY2lPaUpTVXpJMU5pSXNJbXRwWkNJNklrNVhjRkJvV2taMmRsOUxkVWxwUkVSS1RsRjJWMGh2UWt4MGVVdFFjM3B0WW1SbE9WWm9RV3RGVlZVaWZRLmV5SnBjM01pT2lKcmRXSmxjbTVsZEdWekwzTmxjblpwWTJWaFkyTnZkVzUwSWl3aWEzVmlaWEp1WlhSbGN5NXBieTl6WlhKMmFXTmxZV05qYjNWdWRDOXVZVzFsYzNCaFkyVWlPaUprWldaaGRXeDBJaXdpYTNWaVpYSnVaWFJsY3k1cGJ5OXpaWEoyYVdObFlXTmpiM1Z1ZEM5elpXTnlaWFF1Ym1GdFpTSTZJbVJsWm1GMWJIUXRkRzlyWlc0dGNYb3llSGNpTENKcmRXSmxjbTVsZEdWekxtbHZMM05sY25acFkyVmhZMk52ZFc1MEwzTmxjblpwWTJVdFlXTmpiM1Z1ZEM1dVlXMWxJam9pWkdWbVlYVnNkQ0lzSW10MVltVnlibVYwWlhNdWFXOHZjMlZ5ZG1salpXRmpZMjkxYm5RdmMyVnlkbWxqWlMxaFkyTnZkVzUwTG5WcFpDSTZJbUUzWkRsa1l6WXlMVEV4WWpRdE5EUTRZaTA0TmpCakxUZzFaalppTWpkak1UZGpOQ0lzSW5OMVlpSTZJbk41YzNSbGJUcHpaWEoyYVdObFlXTmpiM1Z1ZERwa1pXWmhkV3gwT21SbFptRjFiSFFpZlEuWFZ0bXh5bkFPMnVjMHRLYUJweHV1dVlqbGJYQklFel9YUFJPcnE2LVJqNXNsT3l3WGJCMzFDZGhRS0FfYVA4SUpQRmhUbFE0TzVtMmZNTnUyS2dyYW9qUXdFWGoyMGdxVGJyNVY3RU1fVXNLOFBZZEs4QUZwSlhEWWszZ1RtTV96MUFtNDI2REoyQllpNWU5eDItYUFZRWhoT0I3S1RpY19WQUtaTmtQNWFjSERHYTdOckFGTjg4ZTNyZnpGRURUODZfVVJKV0NiT1dnZ2E2TV9EdFlwcHdSTWpxZHM1Mi1aWFd5bnZGZ25FVGhueGhEck9SOHFEZWxOQk1hOUdxZERybW9YNkVQazd3dWpWZ1ppcGRvV2ptMFZLXzd3VXR2dU93WWRjZmNkNHNDQnhuR1ZWbmY1bld6VS13X0FBS3ZFaDR1dGx4TTZLY2EtMDNTYU1KTmdB --server apiserver.hostname.local
                kubectl apply -f service.yaml --token ZXlKaGJHY2lPaUpTVXpJMU5pSXNJbXRwWkNJNklrNVhjRkJvV2taMmRsOUxkVWxwUkVSS1RsRjJWMGh2UWt4MGVVdFFjM3B0WW1SbE9WWm9RV3RGVlZVaWZRLmV5SnBjM01pT2lKcmRXSmxjbTVsZEdWekwzTmxjblpwWTJWaFkyTnZkVzUwSWl3aWEzVmlaWEp1WlhSbGN5NXBieTl6WlhKMmFXTmxZV05qYjNWdWRDOXVZVzFsYzNCaFkyVWlPaUprWldaaGRXeDBJaXdpYTNWaVpYSnVaWFJsY3k1cGJ5OXpaWEoyYVdObFlXTmpiM1Z1ZEM5elpXTnlaWFF1Ym1GdFpTSTZJbVJsWm1GMWJIUXRkRzlyWlc0dGNYb3llSGNpTENKcmRXSmxjbTVsZEdWekxtbHZMM05sY25acFkyVmhZMk52ZFc1MEwzTmxjblpwWTJVdFlXTmpiM1Z1ZEM1dVlXMWxJam9pWkdWbVlYVnNkQ0lzSW10MVltVnlibVYwWlhNdWFXOHZjMlZ5ZG1salpXRmpZMjkxYm5RdmMyVnlkbWxqWlMxaFkyTnZkVzUwTG5WcFpDSTZJbUUzWkRsa1l6WXlMVEV4WWpRdE5EUTRZaTA0TmpCakxUZzFaalppTWpkak1UZGpOQ0lzSW5OMVlpSTZJbk41YzNSbGJUcHpaWEoyYVdObFlXTmpiM1Z1ZERwa1pXWmhkV3gwT21SbFptRjFiSFFpZlEuWFZ0bXh5bkFPMnVjMHRLYUJweHV1dVlqbGJYQklFel9YUFJPcnE2LVJqNXNsT3l3WGJCMzFDZGhRS0FfYVA4SUpQRmhUbFE0TzVtMmZNTnUyS2dyYW9qUXdFWGoyMGdxVGJyNVY3RU1fVXNLOFBZZEs4QUZwSlhEWWszZ1RtTV96MUFtNDI2REoyQllpNWU5eDItYUFZRWhoT0I3S1RpY19WQUtaTmtQNWFjSERHYTdOckFGTjg4ZTNyZnpGRURUODZfVVJKV0NiT1dnZ2E2TV9EdFlwcHdSTWpxZHM1Mi1aWFd5bnZGZ25FVGhueGhEck9SOHFEZWxOQk1hOUdxZERybW9YNkVQazd3dWpWZ1ppcGRvV2ptMFZLXzd3VXR2dU93WWRjZmNkNHNDQnhuR1ZWbmY1bld6VS13X0FBS3ZFaDR1dGx4TTZLY2EtMDNTYU1KTmdB --server apiserver.hostname.local
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
