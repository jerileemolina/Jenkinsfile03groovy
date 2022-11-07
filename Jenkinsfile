pipeline {
    agent any
    stages {
        stage("release groovy") {
            steps{
                echo "SIN BASH bucle.........................."
                script {
                    def release = readYaml (file: 'release.yml')
                    //para saber que tipo de variable es
                    println release.getClass().getName()
                    release.each{k,v->
                        println "La versión de " + k + " es: " + v
                    }
                }
            }
        }
    }
}