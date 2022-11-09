pipeline {
    agent any
    stages {
        stage("release groovy") {
            steps{
                echo ""
                script {
                    //sacar contenido del release.yml en una variable release
                    def release = readYaml (file: 'release.yml')
                    //para saber que tipo de variable es (la variable es tipo de HashMap)
                    println release.getClass().getName()
                    // Cambio valores de la variable release (tipo HashMap)
                    release.put("APP_JAVA_INT", '0.0.10')
                    println("La versión de APP_JAVA_INT ahora es: "+release);

                    //Mostrar que ha hecho el cambio en la variable
                    release.each{k,v->
                        println "La versión de " + k + " es: " + v

                    // Meter los datos de la variable en un archivo nuevo llamado igual, y lo sobreescribe
                    //WriteYaml Overwrite)




                    }
                }
            }
        }
    }
}