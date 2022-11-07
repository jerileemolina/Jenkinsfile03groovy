pipeline {
agent any 
   stages {
       stage ('Ejercicio 3') {
      steps {
        echo "Ejercicio 3 con groovy"
        script{
          File archivo = new File('release.yml')
          archivo.eachLine { linea ->
             println linea 
                    }
                }
            }
        }
    }
}