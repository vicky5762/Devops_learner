pipeline {
agent any

```
triggers {
    githubPush()
    pollSCM('H/2 * * * *')
}

stages {

    stage('Checkout') {
        steps {
            echo "Cloning repository..."
            git 'https://github.com/vicky5762/Devops_learner.git'
        }
    }

    stage('Build') {
        steps {
            echo "Build Stage Running"
            sh 'java -version'
        }
    }

    stage('Test') {
        steps {
            echo "Testing Stage Running"
            sh 'echo Running tests...'
        }
    }

    stage('Deploy') {
        steps {
            echo "Deployment Stage"
            sh 'echo Application deployed successfully'
        }
    }

}

post {
    success {
        echo "CI/CD Pipeline completed successfully"
    }
    failure {
        echo "Pipeline failed"
    }
}
```

}
