pipeline {
    agent any
    tools {
    maven 'maven-3.6.3' 
  }
    stages {
         
        stage("Build"){
            steps{
                sh "mvn -DskpTests clean package"
            }
        }
        
        stage("Tests"){
            steps{
                sh "mvn test"
            }
        }
    }
}
