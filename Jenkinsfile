pipeline {
    agent any
    stages {
        stage('vcs') {
            steps {
                git url: 'https://github.com/saipurna998/spring-petclinic.git',
                    branch: 'main'
            }
        }
        stage('build') {
            steps {
                sh 'mvn package'
            }
        }
    }
}