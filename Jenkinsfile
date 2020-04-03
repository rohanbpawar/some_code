pipeline {
 agent any
 environment{
  NEW_VERSION = '1.3.0'
 }
 stages{
  stage("build"){
    steps{
      echo 'building the application' 
      echo "version number is ${NEW_VERSION}"
      withCredentials([
       usernamePassword( credentials:'test', usernameVariable: USER , passwordVariable: PASSWORD)
      ])
     {
      echo "${USER} ${PASSWORD}"
     }
     }
    }
  stage("test"){
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
