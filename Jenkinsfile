
pipeline{
    agent any

    stages{
        stage('git checkout'){
            steps{
                git  'https://github.com/OmarAZ1509/hello-world-spring-boot.git'
            }
        }
        stage('build the application'){
            steps{
                bat 'mvn clean install'
            }
        }
            stage('Unit Test Execution') {
            steps{
                bat 'mvn test'
            }
        }
        stage('package') {
            steps {
                bat 'mvn package'
            }
        }
    }
}
