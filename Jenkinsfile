pipeline {
    agent any
    
    stages{
        stage('Build docker image'){
            steps{
                script{
                    sh 'docker build -t baxxah/intern_app .'
                }
            }
        }
        stage('Push image to Hub'){
            steps{
                script{
                   sh 'docker login -u baxxah-p Do42615185'  
                   }
                   sh 'docker push baxxah/intern_app'
                }
            }
        }
        
    }