pipeline { 
    agent any
    stages {
        stage('Clone Git') {
            steps {
                git 'https://github.com/SilverSurge/SummationPipeline.git'
            }
        }
        stage('Build Code') {
            steps {
                sh "chmod u+x Summation.py"
                sh "./Summation.py"
            }
        }
     stage('Test Code') {
            steps {
                sh "chmod u+x Test.py"
                sh "./Test.py"
            }
        }
    } 
}