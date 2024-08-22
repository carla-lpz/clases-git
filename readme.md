# Clase 01 - Git Desarrollo Colaborativo

## Verificando que tenga git instalado

```sh
git --version
```

## Ver si tengo un usuario y correo configurado

```sh
git config --get-regexp user
```

## Configuración inicial

```sh
git config --global user.name "Carla Lopez"
git config --global user.email lpz.carla12@gmail.com
```

## Cómo remover algo que deseo que no esté:

```sh
git config --global --unset user.email
```

## Para cambiar el editor:

```sh
git config --global core.editor <editor>
```

## Cambiar el nombre por defecto de la rema principal

```sh
git config --global init.defaultBranch main
```

## Ver configuraciones hechas en un editor

```sh
git config --global -e
```

## Inicializar un repositorio en GIT

```sh
git init
```
Creará una carpeta .git donde se cuadará el repositorio.

## Para ver las carpetas y archivos ocultos en linux

```sh
ls -la
``` 
## Ver el estado de los archivos del proyecto

```sh
git status
```
Archivos que están "untracked" o sea sin seguimiento.

## Areas posibles en las que pueden estar los archivos

* Working Directory (directorio de trabajo) donde van agregando, borrando al archivo en desarrolo
* Staging Area (área de control de cambios) Se agregan los archivos para darle seguimiento y posteriormente sacarles una foto (commit)
* Local Repo (area de validación de cambios, donde se registrna las modificaciones realizadas) Donde van a estar todas las fotos (commits) que vaya sacando.

## Estados de los archivos

* Untracked (sin seguimiento) > archivos que no se agregaron al intex/stage y por consecuente no se les da seguimiento
* Staged > Archivos que fueron agregados al index/stage area y cuyos cambias van a ser incorporados al repositorio.
* Unmodified > Archivos que se encuentran en el repositorio y no fueron modificados (con respecto al repositorio).
* Modified > Archivos que se encuentran en el repositorio pero difieren con lo que se encuentra actualmente en el directorio de trabajo (working directory).