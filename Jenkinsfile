pipeline {
    agent any

    stages {
        stage('List WorkSpace') {
            steps {
                echo 'Listing WorkSpace..'
                sh 'ls'
                
            }
        }

        stage('Find the OS') {
            steps {
                 sh 'uname -a'
                 sh  'mvn -v'
            }               
        }
    }
}
