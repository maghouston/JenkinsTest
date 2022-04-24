pipeline {
    agent any
    tools {
    maven 'maven' 
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
