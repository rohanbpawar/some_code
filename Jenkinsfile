pipeline {
 agent any
 environment{
  NEW_VERSION = '1.3.0'
  SERVER_CREDENTIALS = credentials('test')
 }
 stages{
  stage("build"){
    steps{
      echo 'building the application' 
      echo "version number is ${NEW_VERSION}"
      echo " ${SERVER_CREDENTIALS} "
     }
    }
  stage("test"){
    steps{
      echo ' bn the application'  
     }
    }
  stage("deploy"){
    steps{
     echo 'deploy the application'  
    }
   }
  }  
 }
