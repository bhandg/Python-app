@Library("Shared") _
pipeline{
    agent { label "gorakh" }
    stages {
        stage('Hello'){
            steps{
                script{
                    hello()
                }
            }
        }
        stage('checkout'){
            steps{
                script{
                    clone("https://github.com/bhandg/Python-app.git","dev")
                }
            }
        }
        stage('build'){
            steps{
                echo " build using maven"
            }
        }
        stage('test'){
            steps{
                echo " code successfully tested on UAT "
                
            }
        }
        stage('deploy'){
            steps{
                echo "deploy on kubernities"
            }
        }
        
    }
    
}
