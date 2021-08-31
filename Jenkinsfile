pipeline{

    agent any

    tools{
        maven 'Maven 3.8.2'
    }
    stages{

        stage('build app'){
            steps{
                sh 'mvn compile'
            }
        }

        stage('test app'){
            steps{
                sh 'mvn clean test'

            }
        }

        stage('package'){
            steps{
                sh 'mvn package -DskipTests'
            }
        }
    }
}