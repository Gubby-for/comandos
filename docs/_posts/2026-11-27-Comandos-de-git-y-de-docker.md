---
layout: post
title:  "Comandos de git y docker"
---

## Comandos de github 

| Comando | Descripción y funcionamiento |
| :---- | :---- |
| **git init** | Inicializa un nuevo repositorio |
| **git clone \<url\>** | Hace una copia 1:1 de nuestro repositorio a nuestro equipo mediante una url |
| **git remote \-v** | Muestra las direcciones URL de los repositorios remotos , e indica la ruta de descarga (fetch) y de subida (push) |
| **git remote add origin \<url\>** | Conecta nuestro repositorio local remoto asignandole|
| **git status** | Muestra el estado actual de los archivos  |
| **git diff** | Muestra las diferencias exactas línea por línea. |
| **git add \<archivo\>** | Añade un archivo específico |
| **git add .** | Agrega todos los archivos nuevos o modificados del directorio actual |
| **git restore \--staged \<archivo\>** | Saca un archivo ya rastreado del área de preparación  |
| **git rm \--cached \<archivo\>** | Elimina un archivo nuevo del área de preparación |
| **git commit \-m "\<mensaje\>"** | Guarda una instantánea permanente de los cambios preparados con mensaje descriptivo. |
| **git log** | Muestra el historial de commits |
| **git push** | Envía los commits guardados en la rama local. |
| **git push \-u origin \<rama\>** | Publica una rama local en el repositorio remoto 'origin' |
| **git pull** | Descarga los cambios recientes desde el repositorio remoto |
| **git stash** | Guarda temporalmente los cambios locales no confirmados (de archivos rastreados) en una pila oculta |
| **git stash save "\<mensaje\>"** | Guarda los cambios locales en un nuevo stash. |
| **git stash push / git stash \-m "\<mensaje\>"** | Sintaxis moderna equivalente a stash save para guardar cambios temporales con un mensaje opcional. |
| **git stash \-u** | Guarda en el stash los cambios incluyendo también los archivos nuevos que aún no están rastreados por Git (untracked). |
| **git stash \-a** | Guarda en el stash todos los cambios, incluyendo archivos no rastreados e incluso archivos ignorados en .gitignore. |
| **git stash list** | Muestra la lista completa de todos los stashes almacenados. |
| **git stash apply** | Recupera y aplica los cambios del stash a la rama actual. |
| **git stash pop** | Recupera y aplica los cambios del último stash (o el indicado) a la rama actual y lo elimina de la pila. |
| **git stash drop \<stash\>** | Elimina un stash específico de la lista cuando ya no se necesita (ej. git stash drop stash@{0}). |
| **git stash clear** | Elimina por completo todos los stashes almacenados en el repositorio. |
| **git branch** | Lista todas las ramas locales del repositorio e indica en cuál nos encontramos situados actualmente. |
| **git branch -a** | Lista tanto las ramas locales como las ramas remotas existentes. |
| **git checkout -b <nueva-rama>** | Crea una nueva rama de trabajo independiente (ej. `git checkout -b mejora-readme`) y cambia automáticamente a ella. |
| **git switch -c <nueva-rama>** | Alternativa moderna a `checkout -b` para crear una nueva rama y posicionarse en ella inmediatamente. |
| **git checkout <otra-rama>**  | Cambia el directorio de trabajo a otra rama existente (ej. `git checkout main`). |
| **git switch <otra-rama>**  | Alternativa moderna a `checkout` para cambiar de una rama a otra. |
| **git branch -m <nuevo-nombre>**  | Renombra la rama en la que nos encontramos situados actualmente. |
| **git branch -d <rama>**  | Elimina una rama local que ya ha sido fusionada previamente. |
| **git merge <otra-rama>**  | Fusiona el historial y los cambios de la rama indicada (`<otra-rama>`) dentro de la rama en la que estamos situados actualmente. |

## Comandos de Docker 

| Comando | Descripción y funcionamiento |
| :---- | :---- |
| **docker run \<imagen\>** | Crea y ejecuta un contenedor a partir de una imagen (ej. docker run redis). |
| **docker ps** | Muestra los contenedores que se encuentran actualmente en ejecución. |
| **docker build** | Construye una nueva imagen de Docker a partir de las instrucciones definidas en un archivo Dockerfile. |
| **docker push** | Sube nuestras propias imágenes locales hacia un registro como Docker Hub para almacenarlas o compartirlas. |
| **docker compose up** | Lee el archivo docker-compose.yml, levanta, crea e interconecta todos los servicios. |