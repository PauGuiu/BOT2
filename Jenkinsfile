pipeline {
  agent any
  stages {
    stage('paso 1') {
      steps {
        echo 'test1'
      }
    }

    stage('paso 2') {
      steps {
        fileExists 'bot2'
        sh '''#!/bin/bash 




# Guardar el nombre del archivo que queremos 
leer archivo_original="$1"
 # Guardar el nombre del nuevo 
archivo archivo_nuevo="$2" 
# Leer el archivo original 
codigo_original=$(<$archivo_original) 
# Escribir el código en el nuevo archivo 
echo -e "$codigo_original" > $archivo_nuevo 
# Mostrar un mensaje de éxito 
echo "El archivo \'$archivo_nuevo\' ha sido creado con éxito con el mismo código del archivo \'$archivo_original\'"'''
      }
    }

  }
}