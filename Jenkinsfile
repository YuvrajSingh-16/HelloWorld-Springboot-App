pipeline{
    agent any
    stages{
        stage('Git clone'){
            steps{
                git 'https://github.com/YuvrajSingh-16/HelloWorld-Springboot-App'
            }
        }
        
        stage('Maven Test'){
            steps{
                bat 'mvn test'
            }
        }
        
        stage('Maven Build'){
            steps{
                bat 'mvn package'
            }
        }
        
        stage('Maven Deploy'){
            steps{
                echo "[+] Deploying war file to the server"
            }
        }
    }
}
