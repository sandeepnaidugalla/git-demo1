pipeline {
    agent any

    stages {
        stage('Git Clone') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/sandeepnaidugalla/git-demo1.git']]])
                echo 'Cloning Git'
            }
        }
        stage('Sandeep') {
            steps {
                bat 'python sandeep.py'
                
            }
        }
        stage('Deepu') {
            steps {
                bat 'python deepu.py'
            
            }
        }
    }
}
