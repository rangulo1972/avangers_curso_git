pipeline {
    agent any


    stages {
        stage('Detectar commits en mi repositorio') {
            steps {
               script {
                def mensajeDelCommit = sh(
                    script: "git log -1 --pretty=%B",
                    returnStdout: true
                ).trim()

                echo "El ultimo commit tiene el siguiente mensaje: ${mensajeDelCommit}"
               }
            }
        }
    }
}
