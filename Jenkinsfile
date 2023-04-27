pipeline {
    agent any 
    stages{
        stage("Source Code Management"){
            steps{
                git branch: 'main', url: 'https://github.com/amitmaurya07/Jenkins_prac.git'
            }
        }

        stage('SonarQube Analysis'){
            def scannerhome= tool ('sonarqube')
            withSonarQubeEnv('sonarqube-token'){
            }
        }
    }
}