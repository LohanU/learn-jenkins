pipeline {
    agent {
        label 'AGENT-1'
    }
    options{
        timeout(time: 10, unit: 'SECONDS')
    }
    stages {
        stage('Build') { 
            steps {
                
                    sh 'echo this is build'
                    sh 'sleep 10'
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
                    //error 'pipeline failed'
                }  
            
            
        }
    
 }
 post {
    always {
        echo "This sections runs always"
        deleteDir()
    
    }
    success{
        echo "this sections runs when pipeline success"
    }
    failure{
        echo "this sections runs when pipeline failure"
    }

 }

}
