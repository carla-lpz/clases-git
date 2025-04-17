# Clase 03

## Ramas (Branches)
![estructuras-ramas]()

## Creando una rama
```sh
git branch <nombre-rama>
```

## Crear rama y moverse a esa rama
```sh
git switch <nombre-rama>
git switch feature/ramas
git switch - #toggle entre las 2 ultimas ramas en las que estuve
git switch -c #crea la rama y te mueve a esa misma rama nueva que creaste.
```
## HEAD : indica en qué rama estoy parado 

## Para borrar ramas

```sh
git branch -d <nombre-rama> # elimina la rama que está mercheada
git branch -D <nombre-rama> # elimina la rama que no está mercheada
```

 