node{
  stage('SCM Checkout'){
    git 'https://github.com/Preranab-git/TestMaven.git'
  }
  stage('Compile-Package'){
   // get maven home path
    def mvnHome = tool name: 'Maven', type: 'maven'
    sh "${mvnHome}/bin/mvn package"
  }
}
