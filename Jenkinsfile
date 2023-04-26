pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs' 
    }
    

    stages{
        stage('one'){
            steps{
                echo 'this is the Build job'
                sh 'npm install'
            }
        }
        stage('two'){
            steps{
                echo 'this is the test job'
                sh 'npm step'
            }
        }
        stage('three'){
            steps{
                echo 'this is the package job'
                sh 'npm run package'
            }
        }
    }
    
    post{
        always{
            echo 'Shhoping Portal pipeline completed...'
        }
        
    }
    
}

