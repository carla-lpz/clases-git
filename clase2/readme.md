# Clase 02

## Repaso de comandos para realizar persistir los cambios de archivos dentro del repositorio

```sh
git status
git status --short
```

## GIT COMMIT: Para persistir los cambios que elegimos y colocamos en el Staging Area

```sh
git commit -m "correcciones"
```

## Corregir un commit (tanto el mensaje como el contenido)

```sh
git add <nombre-archivo>
git commit --amend
```

## Visualizar el timeline de los snapshots (commits) hechos

```sh
git log # versión larga
git log --oneline # versión corta
git log --oneline -2 # ver una cantidad limitada de commits
```
Nota: para salir de la aplicación "less", apretar tecla "q" de quit.


## Hacer commits de parte de un archivo

![alt text](image.png)

```sh
git add --patch

# Menu interactivo, donde git me va ir preguntando qué quiero hacer con los hunks
# y -> Si quiero marcar hunk para enviar al staging area
# n -> No quiero marcar hunk para enviar al staging area
# s -> split: le propongo a git que intente hacer la división
# e -> Decido yo qué linea quiero enviar al staging area
```

## .gitignore
Archivo para desestimar diferentes capetas y archivos que no quiero que formen parte del repositorio.

```sh
touch .gitignore
```

## Agregando REMOTO
```sh
git remote add <alias> <url>
git remote add origin https://github.com/carla-lpz/clases-git.git ## usen HTML
```

## Ver si tengo un remoto en mi local
```sh
git remote # versión corta
git remote -v # versión detallada
```
## Para subir los cambios
```sh
git push -u <remoto> <rama-loca>
git push -u origin main
```

## Checklist
- [x] si
- [ ] no

## Ver cambios del remoto (trae solo matadata)

```sh
gif fetch
```

## Traer cambio y metadata
```sh
git pull
```



