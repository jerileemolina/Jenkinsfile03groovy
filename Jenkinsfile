pipeline {
agent any 
    stage(Ejercicio3 con groovy)
      steps {
        echo "Ejercicio 3 con groovy"
        script {
          def release = readYaml(file: 'release.yml')
          println release.getClass().getName()
          release.each{k,v->
          println "La versión de " + k + "es: " +v
            }
        }
    }
}