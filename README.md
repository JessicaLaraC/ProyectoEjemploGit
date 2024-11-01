 # Práctica 1: Introducción a Git

## Descripción.
Esta práctica consiste en crear un repositorio de Git, utilizando commits basicos de Git, en la Git Bash. Se creará un archivo en Python (`HolaMundo.py`) . El objetivo es familiarizarse con el uso básico de Git, GitHub.

## Instrucciones de uso.
Para ejecutar el programa `HolaMundo.py`, sigue estos pasos:

1. Asegúrate de estar en la carpeta del repositorio.
2. Ejecuta el siguiente comando:
   
   ```bash
   python HolaMundo.py
   
## Comandos utilizados.
1. Inicializar el repositorio
   
   ```
   git init
   ```
   
3. Crear el primer commit en el archivo `HolaMundo.py`
   
   ```
   git add HolaMundo.py
   git commit -m "Se agregó el programa de Hola en Python"
   ```
   
4. Crear el segundo commit en el archivo `.gitignore`
   
   ```
   git add .gitignore
   git commit -m "Se agregó el archivo .gitignore"
   ```
5. Verificar que debug.log es ignorado

     ```
     git status --ignored
      ```
     
6. Conectat el repositorio local a GitHub y subir los cambios
   
   ```
   git remote add origin https://github.com/JessicaLaraC/ProyectoEjemploGit.git
   git push -u origin main
    ```

## Archivo `.gitignore`
El archivo `.gitignore` se creó para evitar que ciertos archivos se suban al repositorio remoto en GitHub. Esto es útil para archivos que no forman parte del código fuente, como archivos de registro (`.log`), configuraciones locales o archivos temporales. En este caso, se ignoran todos los archivos con extensión `.log`, incluyendo `debug.log`.

Para verificar que `debug.log` no se subió al repositorio en GitHub, puedes revisar los archivos en el repositorio remoto y confirmar que `debug.log` no está en la lista. Esto confirma que `.gitignore` está funcionando correctamente.

## Descripción de la salida del programa
Al ejecutar `HolaMundo.py`, el programa debe mostrar el mensaje:

 ```
Hola Git
 ```
