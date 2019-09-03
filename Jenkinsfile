pipeline {
    agent any
    stages {
        stage ('Testing Jenkinsfile') {
            steps {
                echo 'Probando conexion a google'
                sh 'ping -c 10 www.google.com && sleep 5'
                echo 'Imprimir variables de entorno'
                sh 'set | sort' // se ocupa set, pero tb puede ser "printenv" o "env"
                echo 'Imprimir Helloworld'
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

