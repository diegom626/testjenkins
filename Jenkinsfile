pipeline {
    agent any
    stages {
        stage ('Testing env') {
            steps {
                echo 'Probando conexion a google'
                sh 'ping -c 10 www.google.com'
                sleep 10
                echo 'Imprimir variables de entorno'
                sh 'set'
                echo 'Helloworld'
                sh 'Hello world!! mi user es $(whoami)'
            }
        }
    }
}