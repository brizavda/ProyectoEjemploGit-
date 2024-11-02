
# Práctica 1: Introducción a Git

## Descripción
En esta práctica, se desarrolla un programa básico en Python, `HolaMundo.py`, que imprime un mensaje en la consola. El objetivo es aprender a utilizar los comandos básicos de Git, crear un repositorio local y remoto en GitHub, y gestionar el archivo `.gitignore` para controlar qué archivos deben ser ignorados en el repositorio.

## Instrucciones de Uso
1. Clona el repositorio o accede al directorio donde está el archivo `HolaMundo.py`.
2. Ejecuta el programa con el siguiente comando:
   ```bash
   python HolaMundo.py
   ```

## Comandos Utilizados
- `git init`: Inicializa un nuevo repositorio en la carpeta `ProyectoEjemploGit`.
- `git add <file>`: Añade archivos al área de preparación (staging).
- `git commit -m "mensaje"`: Crea un commit con los archivos añadidos.
- `git status`: Muestra el estado de los archivos en el repositorio.
- `git remote add origin <URL>`: Conecta el repositorio local a un repositorio remoto.
- `git push origin main`: Sube los cambios al repositorio remoto en GitHub.

## Notas sobre el archivo `.gitignore`
- **Propósito**: El archivo `.gitignore` se creó para excluir archivos innecesarios del repositorio, en este caso, archivos de prueba o de registro (logs).
- **Archivos ignorados**: Se ignoran todos los archivos con la extensión `.log`, como `debug.log`.

## Verificación
Al ejecutar `HolaMundo.py`, el programa debe mostrar:
```plaintext
Hola Mundo
```
En el tercer paso, el mensaje debe actualizarse a:
```plaintext
Hola Git
```
Para asegurarse de que `debug.log` no se subió, usa el comando:
```bash
git status
```
Este comando debería indicar que `debug.log` no está en el área de preparación ni aparece como archivo no rastreado.
```
