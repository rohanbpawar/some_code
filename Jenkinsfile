pipeline {
 agent any
 parameters{
  string( name: 'NEW_VERSION', defaultValue:'1.23.1', description: '')
 }
 stages{
  stage("build"){
    steps{
      echo 'building the application' 
      echo "version number is ${NEW_VERSION}"
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
