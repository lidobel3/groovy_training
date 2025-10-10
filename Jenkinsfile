pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'mkdir ./TOTO' //Jenkins va créer le repertoire dans /var/jenkins_home/workspace/apprentissage/TOTO 
            }
        }
        stage('Test') {
            steps {
                echo 'Exécution des tests...'
            }
        }
    }
}
