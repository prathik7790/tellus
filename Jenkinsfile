node {
  echo 'Hello World'
  stage('Code Checkout'){
  checkout scm
  }
  stage('Maven'){
  sh 'export MAVEN_HOME=/opt/maven'
  sh 'export PATH=$PATH:$MAVEN_HOME/bin'
  sh 'mvn --version'
  sh 'mvn clean package'
  }
  stage('Build') {
        
      dir ('tellus') {
            sh 'mvn clean install test'
      } 
       
   }
}
