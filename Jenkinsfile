pipeline {
 agent any
 stages{
  stage("build"){
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
