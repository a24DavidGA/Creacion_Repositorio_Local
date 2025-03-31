pipeline {
    agent none
    
    stages {
        stage("Build and Test the Project") {
            agent {
                docker {
                    image 'python:2'
                }
            }
            
            stages {
                stage('En el Contenedor') {
                    steps {
                        sh 'python --version'
                    }
                }
            }
        }
        
        stage("Deploy in Production") {
            agent any
            
            stages {
                stage('En la Máquina') {
                    steps {
                        sh 'python3 --version'
                    }
                }
            }
        }
    }
}
