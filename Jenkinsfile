triggers {
    githubPush()
    pollSCM('H/2 * * * *')
}

stages {

    stage('Checkout') {
        steps {
            git 'https://github.com/vicky5762/Devops_learner.git'
        }
    }

    stage('Build') {
        steps {
            sh 'java -version'
        }
    }

    stage('Deploy') {
        steps {
            sh 'echo Deploying application'
        }
    }

}