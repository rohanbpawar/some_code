pipeline {
 agent any
 stages{
  stage("build"){
    when{
     expression {
      BRANCH_NAME == "master"  && CODE_CHANGE == true
      }
     }
    steps{
      echo 'building the application'  
      }
    }
  stage("test"){
    when{
     expression {
       BRANCH_NAME == "dev" 
      }
     }
    steps{
      echo 'test the application'  
     }
    }
  stage("deploy"){
    steps{
     echo 'deploy the application'  
    }
   }
  }  
 }
