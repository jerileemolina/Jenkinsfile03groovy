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
                    // modificar valores de yaml
                    prop.setProperty("k", "v");
                    prop.setProperty("APP_JAVA_INT", "0.0.5");
                        println " La versión de " + k + "ahora es:" + def var = null
                    }
                }
            }
        }
    }
}