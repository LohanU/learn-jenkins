pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                
                    sh 'echo this is build'
                } 
            
        }
        stage('Test') { 
            steps {
               
                    sh 'echo this is test'
                }  
            
        }
        stage('Deploy') { 
            steps {
               
                    sh 'echo this is deploy'
                    error 'pipeline failed'
                }  
            
            
        }
    
 }
 post {
    always {
        echo "This sections runs always"
    
    }
    success{
        echo "this sections runs when pipeline success"
    }
    failure{
        echo "this sections runs when pipeline failure"
    }

 }

}
