pipeline {
    agent any
    stages {
        stage("release groovy") {
            steps{
                echo ""
                script {
                    def release = readYaml (file: 'release.yml')
                    //para saber que tipo de variable es
                    println release.getClass().getName()
                    release = release.replace('0.0.5', '0.0.10')
                    println release
                    release.each{k,v->
                        println "La versión de " + k + " es: " + v

                    }
                }
            }
        }
    }
}