pipeline {
    
    agent any
    tools { maven "maven3" }
    
    stages {
        
        stage("checkout") {
            
            steps {
                
                git branch: "main", url: "https://github.com/neo3matrix/SpringRESTful.git"
                
            }
        }
        
        stage("build") {
            
            steps {
                
                sh "mvn compile"
            }
        }
        
        stage("test") {
            
            steps {
                
                sh "mvn test"
            }
        }
    }
}
