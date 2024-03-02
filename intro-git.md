# Aprendiendo _GIT_

## Comandos de la Configuración Global

Estos comandos los ejecutas la primera vez que vas a conbfigurar tu información en la computadora donde trabajarás con _GIT_.

```bash
git --version
git config --global user.name "Jonathan MirCha"
git config --global user.email jonmircha@gmail.com
git config --global user.ui true
git config --global init.defaultBranch main
git config --list
# asignando visual studio code como editor de configuración de git
git config --global core.editor "code --wait"
git config --global -e
# para estandarizar los saltos de línea en windows
git config --global core.autocrlf true
# para estandarizar los saltos de línea en linux/mac
git config --global core.autocrlf input
# ver todas las opciones de la configuración en la terminal
git config -h
# ver todas las opciones de la configuración en el navegador
git help config
```

## Flujo Básico de _GIT_

![Flujo Básico de _GIT_](https://jonmircha.com/img/blog/git-flow.png)

## Inicializar _GIT_ por primera vez

```bash
# git init, se ejecuta una sola vez en cada carpeta, para indicarle a git que tiene que supervisar dicha carpeta
git init
# git status, sirve para revisar el estado de los archivos de la carpeta que git esta supervisando
git status
# git log, visualiza el historial de cambios del repositorio
git log


# agregar los cambios de un archivo al staged
git add archivo/directorio
# agregar todos los cambios de todos los archivos al staged
git add .
# saca del stage y regresa al working directory el archivo indicado
git rm --cached archivo
# git commit, es el comando que me permite pasar del stagind al HEAD del repositorio, con este comando oficializo un cambio en el historial de mi repositorio
git commit
git commit -m "Mensaje del commit"
```
