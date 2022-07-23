# CLASE 02

## .gitignore
Es un archivo. Me permite descartar archivos. Que git ignore el archivo.
Se crea normalmente en el directorio raiz del proyecto.

## .gitkeep
Le permite a git ver carpetas vacías y versionarlas

## GIT BRANCH (RAMAS)

### CREAR RAMA
git branch <nombre-rama>
git branch rama-dev

### LISTAR RAMAS
git branch

## CAMBIARME DE RAMA
git switch <nombre-rama>
git switch rama-dev

## GIT MERGE: fusión de ramas
**IMPORTANTE:** Tengo que estar en la rama en la cual quiero traerme los cambios. Si quiero traerme lo rama-branches. Tengo que estar en master y ejecutar el git merge.

git merge <rama-que-me-quiero-traer>
git merge rama-branches

### TIPO DE FUSIONES (MERGE)
fast-forward: (la fusión va a ser automática) No hay conflicto
Recursiva: (Unión automática) No hay conflicto
Manual: (No va poder resolver en forma automática) o sea, hay conflictos.

## GIT LOG
git log --help

git log --oneline --decorate --all --graph


## Agregar Alias
git config --global alias.l "log --oneline"
git config --global alias.l "log --oneline --all --decorate --graph"
git config --global alias.c "commit -am"
git config --global alias.s status --short

## Borrar alias
git config --global --unset alias.c

## Listar alias disponibles
git config --get-regexp alias

## GIT COMMIT (Cont...)
# Enmendar un commit. Corregir.
git commit --amend 
