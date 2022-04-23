pipeline {
    agent any
    tools { 
        maven 'Maven 3.8.5' 
    }
    stages {
        stage("Build"){
            steps{
                sh 'mvn -DskpTests clean package'
            }
        }
        
        stage("Tests"){
            steps{
                sh 'mvn test'
            }
        }
    }
}
