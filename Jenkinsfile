pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                parallel(
                    build: {
                        echo 'Building..'
                    },
                    test: {
                        echo 'Testing..'
                    }
                )
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
