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

    agent {
        docker {
            image 'maven:3.8.8-openjdk-17'
            args '-v $HOME/.m2:/root/.m2' // Pour le cache Maven
        }
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
