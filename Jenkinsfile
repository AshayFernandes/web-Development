pipeline {
  
   agent any
   
   stages {
    
     stage("build") {
       
         steps {
           def pw = pwd()
           echo "building the application..${pw}"
           
         }
     
     }
     
     stage("test") {
       
         steps {
           echo "testing the application.."
         }
     
     }
     
     stage("deploy") {
       
         steps {
           echo "deploying the application.."
         }
     
     }
   
   
   }

}
