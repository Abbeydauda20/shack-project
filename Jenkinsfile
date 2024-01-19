pipeline {
    agent any
    
    tools { maven 'maven3.6'
            jdk 'jdk11'
            
    }

    stages {
        stage('git checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Abbeydauda20/shack-project.git'
            }
        }
        
        stage('Compile') {
            steps {
                sh "mvn compile"
                
            }
        }
        
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        
        
    }
}
