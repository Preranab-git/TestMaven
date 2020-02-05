node {
   stage('SCM Checkout'){
     git 'https://github.com/Preranab-git/TestMaven.git'
   }
   stage('Compile-Package-create-war-file'){
    // get maven home path
     def mvnHome = tool name: 'Maven', type: 'maven'
     bat "${mvnHome}/bin/mvn package"
   } 
 }
