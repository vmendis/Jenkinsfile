pipeline {
    agent any

    stages {
        stage('List WorkSpace') {
            steps {
                echo 'Listing WorkSpace..'
                sh 'pwd'
                sh 'ls'
                
            }
        }

        stage('Find the OS') {
            steps {
                 sh 'uname -a'
                // sh  'mvn -v'
                // sh  'ansible --version'
            }               
        }
    }
}
