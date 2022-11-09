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
                    release.setProperty("aux", "0.0.2")
                    release.each{k,v->
                        println "La versión de " + k + " es: " + v

                    // modificar valores de yaml
                    //prop.setProperty("k", "v");
                    //prop.setProperty("APP_JAVA_INT", "0.0.5");
                        //println " La versión de " + k + "ahora es:" + v

                    //opcion2
                    //java.io.File, java.lang.String
                    //String newVersion = "0.0.20"
                    //yaml.text = yaml.text.replaceFirst(/version: '.*'/, "version: '${newVersion}'")
                    //println yaml.text
                    //content.replace('0.0.5', '0.0.10');
                        

                    }
                }
            }
        }
    }
}