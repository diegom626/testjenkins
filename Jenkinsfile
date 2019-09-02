pipeline {
    agent any
    stages {
        stage ('Testing env') {
            steps {
                echo 'Probando conexion a google'
                sh 'ping -c 10 www.google.com && sleep 5'
                echo 'Imprimir variables de entorno'
                sh 'set | sort'
                echo 'Helloworld'
                sh 'echo -n "Hello world!, estoy usando $(whoami)"'
            }
        }
    }
    post {
        always {
            echo "Pipeline finalizado"
        }
    }
}


