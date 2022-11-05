pipeline {
    agent {
        label 'linux'
    }
    stages {
        stage('Molecule install') {
            steps{
                sh 'pip install molecule==3.4.0'
                sh 'pip install "ansible-lint<6.0.0"'
                sh 'pip install molecule_docker'
            }
        }
        stage('Molecule test'){
            steps{
                sh 'molecule test -s centos_8'
                cleanWs()
            }
        }
    }
}
