pipeline {
    agent any
    stages {
         stage('Initialize'){
            steps{
                echo "PATH = ${M2_HOME}/bin:${PATH}"
                echo "M2_HOME = /opt/maven/apache-maven-3.6.3"
            }
        }
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
