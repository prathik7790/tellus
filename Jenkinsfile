node {
  echo 'Hello World'
  stage('Code Checkout'){
  checkout scm
  }
  stage('Build') {
        
      dir ('tellus') {
            sh 'mvn clean install test'
      } 
       
   }
}
