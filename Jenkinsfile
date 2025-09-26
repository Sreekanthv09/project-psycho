pipeline{
    agent any
    stages {
        stage("SCM Checkout"){
            when {
                branch "develop"
            }
            steps {
                echo "Git checkout successful"
            }
        }
        stage("Maven Build"){
            when {
                branch "develop"
            }
            steps {
                echo "Build successful"
            }
        }
        stage("Dev deploy"){
            when {
                branch "develop"
            }
            steps {
                echo "Deploy to develop"
            }
        }
        stage("Prod deploy"){
            when {
                branch "main"
            }
            steps {
                echo "Deploy to production environment"
            }
        }
    }
}

