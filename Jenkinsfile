node{
  stage('SCM Checkout'){
    git 'https://github.com/Preranab-git/TestMaven.git'
  }
  stage('Compile-Package'){
   // get maven home path
    def mvnHome = tool name: 'Maven', type: 'maven'
    bat "${mvnHome}/bin/mvn package"
    
    properties([parameters([choice(choices: ['master', 'DTPL14'], description: '', name: '')])])
  } 
}
